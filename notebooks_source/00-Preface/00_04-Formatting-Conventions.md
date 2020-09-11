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

## Formatting Conventions

+++

This book and supporting materials use the following formatting conventions.

+++

### Web Address

Web address will be shown as:

 > [https://github.com/professorkazarinoff/Problem-Solving-with-Python](https://github.com/professorkazarinoff/Problem-Solving-with-Python)
 

+++

### Important terms and vocabulary
 
Important terms and vocabulary are shown in _italic text_.

<br>

 > There is a difference between _local variables_ and _global variables_ in Python code.
  

+++

### File Names
 
File names are  shown in **_bold and italic text_**.

<br>

 > After completing the code, save the file as **_hello.py_** in the current directory.

+++

### Module and Package Names
 
Module and Package names will be shown in **bold text**.

<br>
 
 > **NumPy** and **Matplotlib** are two useful packages for problem solvers.
  
 

+++

### Inline code
 
Inline code, including variable names, is shown in ```monospace font```.

<br>
 
 > To compare a variable use ```var == 'string'``` and make sure to include ```==```, the double equals sign.
  

+++

### Separate code blocks
  
Separate code blocks appear in their own sections in ```monospaced font```.

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

+++

### Anaconda Prompt Commands
 
Commands typed into the **Anaconda Prompt** are shown in separate sections which contain the prompt symbol ```>``` before each line. Note the prompt ```>``` should not be typed. The prompt symbol is included to indicate **Anaconda Prompt**, not a character for the user to enter.

```text
> conda create -n env python=3.7
> conda activate env
```

+++

### Terminal Commands
 
Commands typed into the MacOS or Linux terminal appear in separate sections which contain the dollar symbol ```$```  before each line. Note the dollar symbol ```$``` should not be typed. The dollar symbol is included to indicate a terminal prompt, not a character for the user to enter.
 
```text
$ pip install pint
$ cd pint_srcipts
```

+++

### Python REPL Commands

Commands typed into the **Python REPL** (the Python Interpreter) appears in separate code sections, which contain the triple arrow prompt ```>>>``` . Note the triple arrow ```>>>``` prompt should not be typed. Triple arrows are included to indicate the Python REPL prompt, not a character for the user to enter. The output from the Python REPL is shown on a separate line below the command, without the ```>>>``` prompt.

```python
>>> 2 + 2
4
>>> print('Problem Solving with Python')
Problem Solving with Python
```

+++

### Jupyter Notebook cells

Commands typed into Jupyter notebook cells appear with the label ```In [#]:``` to the left of the code section. The output from Jupyter notebook cells is shown below the input cell. Only code in the input cells needs to be typed. Output cell are be produced automatically by clicking the run button or typing ```[shift]+[Enter]```.

```{code-cell} ipython3
A = 2
B = 3
C = A + B
print(C)
```

### Keystrokes and Buttons

Keystrokes directly entered by the keyboard or buttons that are indicated on programs or web pages are shown inside square brackets in ```[monospaced font]```.

<br>

 > In order to delete a line use the ```[Backspace]``` key. To exit the shell type ```[shift]+[c]```

```{code-cell} ipython3

```
