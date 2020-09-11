---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.9'
    jupytext_version: 1.5.0
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

## Uploading Code

+++

In this section, you will learn how to upload code to an ESP8266-based microcontroller with a tool called **ampy**. The code in this section was written to turn the ESP8266-based microcontroller in a scrolling thermometer. The same upload method shown in this section can be used to upload MicroPython code you write to a ESP8266-based microcontroller.

Before MicroPython code is uploaded on the ESP8266-based microcontroller, MicroPython needs to be installed on the board. PuTTY also needs to be installed on you computer in order for the computer to communicate with the microcontroller over a serial connection.

A previous section in this chapter detailed how to install MicroPython on an ESP9266 microcontroller and how to install PuTTY on a Windows. The procedures in this section are specific to the Adafruit Feather Huzzah ESP8266 microcontroller and the MCP9808 temperature sensor, both of which were used in a previous section. Other ESP8266-based microcontrollers and I2C sensors could be used instead, but the specifics of the procedure may be different from what's shown in this section.

+++

### Summary of Steps

+++

1. Install **ampy** with **pip**
2. Write MicroPython code 
3. Upload the MicroPython on code on the microcontroller with **ampy**
4. Unplug and then power up the Feather Huzzah and watch the temperature scroll by

+++

### Install ampy with pip

**Ampy** is a Python package developed by Adafruit, a company that makes MicroPython compatible hardware. **Ampy** is used to push code stored on a computer onto a microcontroller running MicroPython. **Ampy** can be installed using the **Anaconda Prompt**. Alternatively, a terminal can be used to install **ampy**. If you are using a virtual environment, active the virtual environment first then proceed with **ampy** package installation.

+++

```text
> conda activate micropython
(micropython) > pip install adafruit-ampy
(micropython) > ampy --help
```

+++

### Write MicroPython Code

+++

Now write the MicroPython code which you will uploaded on the microcontroller. The Adafruit Feather Huzzah ESP8266 microcontroller contains two main Python files: **_boot.py_** and **_main.py_**. But additional files can also be uploaded to the microcontroller. **_boot.py_** is the file that runs first when the board is powered up. First **_boot.py_** runs, then **main.py** runs. An additional **_.py_** file can be added to the board to provide **_main.py_** with a function to run.

Two different **_.py_** files will be constructed in this section. One **_.py_** file contains a function that reads the temperature off the temperature sensor. A second **_.py_** file calls the function in the first **_.py_** file and prints the temperature to the terminal window with a loop.

+++

The first **_MCP9808.py_** file includes one function called ```readtemp()```. The ```readtemp()``` function reads temperature recorded by the MCP9808 temperature sensor.  The ```readtemp()``` function parses out the temperature data from the I2C bus on the MCP9808 temperature sensor and outputs the temperature in degrees C as a float.

At the top of **_MCP9808.py_** we need to import the ```machine``` module to use the I2C bus. The ```machine``` module provides a class to create a new I2C object. 

When the I2C object is instantiated, the ```scl``` and ```sda``` pins that the MCP9808 temperature sensor is connected to need to be specified. ```scl``` is the I2C clock line and ```sda``` is the I2C data line.  ```scl``` and ```sda```  are pin 5 and pin 4 on the Adafruit Feather Huzzah ESP8266. 

The next part of the ```readtemp()``` function creates a byte array. Data from the MCP9808 temperature sensor will be stored in the byte array. 

The next part of the ```readtemp()``` function in the **_MCP9808.py_** file uses the ```i2c.readfrom_mem_into()``` method to read the temperature off the sensor. The first argument passed to the ```i2c.readfrom_mem_into()``` method is the I2C bus address of the sensor. On the MCP9808 temperature sensor, the I2C bus address is ```24```(if you type the line ```>>> i2c.scan()``` into the MicroPython REPL, the I2C bus address is returned). The next parameter passed to the  ```i2c.readfrom_mem_into()``` method is the register on the MCP9808 temperature sensor where the measured temperature is stored. On the MCP9808, the temperature is stored in register ```5```. The third parameter passed to the  ```i2c.readfrom_mem_into()``` method is the variable we want to store the temperature data in. The ```i2c.readfrom_mem_into()``` method _changes_ the variable passed into the method as the third argument. Most Python methods modify the object the method operates on, but MicroPython's ```i2c.readfrom_mem_into()``` method changes the third variable passed to it, in our case the variable ```byte_data```. That's why we created the ```byte_data``` variable before we called the ```i2c.readfrom_mem_into()``` method. 

The last part of the ```readtemp()``` function includes post-processing needed to convert the byte array into a temperature in degrees C. The final temperature in degrees C is a float

+++

The entire contents of the **_MCP9808.py_** file are below:

```python
# MCP9808.py

# Functions for the  MCP9808 temperature sensor
# learn.adafruit.com/micropython-hardware-i2c-devices/i2c-master

def readtemp():
    import machine
    i2c = machine.I2C(scl=machine.Pin(5), sda=machine.Pin(4))
    byte_data = bytearray(2)
    i2c.readfrom_mem_into(24, 5, byte_data)
    value = byte_data[0] << 8 | byte_data[1]
    temp = (value & 0xFFF) / 16.0
    if value & 0x1000:
        temp -= 256.0
    return temp
```

+++

Now construct a MicroPython script called **_main.py_** which will use the function ```readtemp()``` stored in **_MCP9808.py_**.

The **_main.py_** script will import the **_MCP9808.py_** module and use the ```readtemp()``` function to read the temperature from the MCP9808 temperature sensor. 

Inside **_main.py_** will be a loop that runs  for a total of 120 seconds. Each second the temperature is recorded. Inside the loop, the temperature is read off the MCP9808 temperature sensing using the ```MCP9808.readtemp()``` function.  ```time.sleep(1)``` is inserted into the loop to wait one second between each measurement.

The complete **_main.py_** file is below.

```python
# main.py

import MCP9808
import time

time.sleep(2)

for i in range(120):
    data = MCP9808.readtemp()
    print(data)
    time.sleep(1)
```

+++

### Upload MicroPython Code to the ESP8266 Microcontroller with **ampy**

+++

Once the **_MCP9808.py_** file and the **_main.py_** files are saved, both files can be uploaded on the Adafruit Feather Huzzah ESP8266 microcontroller.

Ensure the microcontroller is connected with a USB cable, and be aware of which serial port the microcontroller is connected to. 

Upload the **_MCP9808.py_** file and the **_main.py_** file to the board using **ampy**. Make sure you are in the directory with the **_.py_** files and that you are working in a virtual environment that has ```ampy``` installed in it. In the example code below, the ```(micropython)``` virtual environment is active. The command ```ampy --port COM4 ls``` lists the files stored on the microcontroller.

```text
(micropython) > ampy --port COM4 put MCP9808.py
(micropython) > ampy --port COM4 put main.py
(micropython) > ampy --port COM4 ls
boot.py
MCP9808.py
main.py
```

+++

### Unplug and then power up the Feather Huzzah and watch the temperature scroll by

+++

The Feather Huzzah needs to be restarted to run the **_main.py_** file uploaded with **ampy**. 

To restart the board, unplug and then replug in the board's power (the USB cable). Once power is restored, the board will run through the **_boot.py_** script then start the **_main.py_** script. When the board runs the **_main.py_** script, the board will read the temperature from the MCP9808 temperature sensor then print the temperature out to the terminal. After two minutes the program should end.

The output below demonstrates the results shown in a terminal window.

```text
...
25.6875
25.75
25.6875
25.6875
25.75
25.6875
25.75
25.75
25.75
25.75
25.75
25.8125
25.8125
25.8125
25.75
25.75
25.8125
>>>
```

```{code-cell} ipython3

```
