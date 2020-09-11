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

+++ {"latex": {"before_cell": "newpage"}}

## Summary

+++

In this chapter, you learned how to use Python to interact with external hardware. In particular, you learned how to use Python and the PySerial package to communicate with an Arduino. 

The chapter began with a discussion of Unicode strings and byte strings. In Python, all strings are Unicode by default, but machines speak in bytes. To create a byte string in Python, prepend a string with the letter ```b``` as in ```b'my string'```. Python's ```.encode()``` and ```.decode()``` methods convert between Unicode strings and byte strings.

In the first project of the chapter, you learned how to use Python and the PySerial package to control an LED attached to an Arduino. The general steps were:
 
 * download and install the Arduino IDE
 * wire a LED to an Arduino
 * connect the Arduino the computer and upload code
 * blink the LED with the Arduino Serial Monitor
 * blink the LED with the Python REPL
 * blink the LED with a Python script
 * run a Python script to have a user turn the LED on and off
 
The second project of the chapter involved reading a sensor connected to an Arduino with Python and PySerial. To complete this project, the general steps were:

 * download and install the Arduino IDE
 * wire a potentiometer sensor and LED to the Arduino
 * connect the Arduino the computer and upload an Arduino sketch
 * check the sensor signal with the LED, Arduino Serial Monitor and Arduino Serial Plotter
 * use the Python REPL to read the potentiometer sensor
 * run a Python script to collect the potentiometer sensor data and plot the data using Matplotlib

+++

### Key Terms and Concepts

+++ {"latex": {"environment": "key_terms"}}

External Hardware

Sensor

LEDArduino

IDE

serial

serial communication

serial line

USB

Unicode

Unicode string

byte string

port

.ino-file

C programming language

baud

newline character

+++

### Additional Resources

The official documentation for the PySerial Package is found here: [https://docs.pyserial.com](#)
    
The Arduino project has a great set of tutorials found here:[https://Arduino.com/tutorials](#)
    
SparkFun has a great overview of wiring an LED to an Arduino here: and a great overview of writing a potentiometer to an Arduino here:

```{code-cell} ipython3

```
