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

## What is MicroPython?

+++

### What is MicroPython?

+++

[MicroPython](http://micropython.org/) is a port, or version of Python designed to run on small, inexpensive, low-power microcontrollers. Examples of microcontrollers that Micropython can run on includes the [pyboard](https://store.micropython.org/), the [WiPy](https://pycom.io/development-boards) and ESP8266-based boards like the [Adafruit Feather Huzzah](https://learn.adafruit.com/adafruit-feather-huzzah-esp8266) and ESP8266 NodeMCU.  

Traditionally, Python runs on desktop or laptop computers and cloud servers. Compared to a desktop or laptop, microcontrollers are much smaller, cheaper and less powerful.  A "regular" version of Python can't run on small, cheap microcontrollers because Python is too resource intensive. Regular Python takes up too much hard disk space, runs on too much RAM and requires a more powerful processor than microcontrollers have. 

It is pretty amazing that a version of Python (MicroPython) runs on these small, cheap microcontrollers like the ESP8266. To get MicroPython to run at all on these little low-cost boards, MicroPython only contains a subset of all the Standard Library modules included with "regular" Python. Some of the libraries that are included with MicroPython don't have the full set of functions and classes that come with the full version of Python. By not including the full functionality of "regular" Python, MicroPython is compact (around 600 kB for the ESP8266 port), and MicroPython only uses a small amount of RAM (down to 16k according to the [Micropython main page](https://micropython.org/).)

You can try using MicroPython online with a browser-based [MicroPython online emulator](https://micropython.org/unicorn/). The emulator allows you to run commands at a MicroPython Prompt and see the result on a virtual pyboard. 

+++

### What is MicroPython used for?

+++

MicroPython can be installed on small, cheap microcontrollers like the [ESP8266](https://learn.adafruit.com/adafruit-feather-huzzah-esp8266). Anything these small microcontrollers can do, MicroPython can do. A microcontroller running MicroPython can read a remote sensor to measure things like temperature, humidity and light level. MicroPython can also be used to blink LED's, control arrays of LED's, or run small displays. MicroPython can control servo motors, stepper motors, and solenoids. Civil Engineers could use MicroPython to monitor water levels. Mechanical Engineers could use MicroPython to drive robots. Electrical Engineers could use MicroPython to measure voltage levels in embedded systems. 

By the end of this chapter, you will learn how to use MicroPython, running on a small cheap ESP8266 board, to turn on and off a light and read a sensor.

+++

### Why should problem solvers learn MircoPython?

+++

Python is used to solve problems such as calculations, statistics, modeling, and visualization. But Python on its own is relatively limited in controlling devices outside the computer it's running on. You don't want to leave a laptop in a remote estuary to measure water temperature, but you could leave a little microcontroller and low-cost temperature sensor in a remote location. A small robot can't carry around a heavy laptop, but a small, light, low-power board could run a simple robot. You don't want to use a computer for every small electrical measurement or embedded system control, but a $2 WiFi module would work. 

Besides, learning how to use MicroPython on small, cheap microcontroller can help problem solvers understand how programming works. Seeing and controlling a motor whirl is a different kind of feedback and excitement compared to seeing text on a screen that shows how fast a motor spins. Seeing an array of LED's light up produces a different kind of wonder compared to seeing a 2-D plot on a computer screen. Plus MicroPython is fun! It's as easy to program MicroPython as it is to program regular Python. The little projects you can do with MicroPython running on a small, low-cost board are almost unlimited. We could send MicroPython to space in a micro-satellite, or bury MicroPython underground in a boring machine, or launch MicroPython into the sky on a weather balloon.

```{code-cell} ipython3

```
