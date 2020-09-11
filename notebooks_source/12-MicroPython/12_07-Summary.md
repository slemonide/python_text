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

In this chapter, you learned about MicroPython. MicroPython is a small slimed down port of the Python programming language designed to run on small cheap microcontrollers. The first part of the chapter introduced MicroPython. "Regular" Python consumes to much hard disk space and RAM to be run installed on a microcontroller. But MicroPython is very small for a programming language. It only takes up less than 1MB on a microcontroller.

The next section of the chapter involved how to install MicroPython on a microcontroller. To install MicroPython on a microcontroller, use a package called **esptool** and upload a .bin firmware file to the board.

The rest of the chapter involved two projects. Blinking an LED with MicroPython and reading a sensor with MicroPython.

To blink an LED on a microcontroller, you need to connect to the microcontroller with a program called PuTTY. Through a PuTTY terminal, you can use MicroPython's ```machine``` module to write high and low values to the pins on the microcontroller. 

An MCP9808 temperature sensor was read using MicroPython in the second project. The sensor first needed to be wired up to the microcontroller, and then the MicroPython's ```ic2``` class was used to read data off the sensor. At the end of the project, a Python package called **ampy** was used to upload a **_.py_** file to the microcontroller.

+++

### Key Terms and Concepts

+++ {"latex": {"environment": "key_terms"}}

MicroPython

microcontroller

MicroPython REPL

REPL prompt

baud rate

port

pyboard

ESP8266

resource intensive

esptool

.bin firmware file

driver

USB data cable

PuTTY

MCP9808 temperature sensor

ampy

Hello World

```{code-cell} ipython3

```
