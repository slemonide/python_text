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

## Review Questions

+++ {"latex": {"environment": "problems"}}

#### Code cells and markdown cells

Q02.01 Run the following code in two different Jupyter notebook cells. Run one cell as a code cell. Run the other cell as a Markdown cell. Why is the output different?

```text
# Problem Solving with Python
```

Q02.02 Run the following code in two different Jupyter notebook cells. Run one cell as a code cell. Run the other cell as a Markdown cell. Why is the output different?

```text
print('Problem Solving with Python')
```

+++ {"latex": {"environment": "problems"}}

#### Markdown cells

Q02.10 Recreate the following headings in one Jupyter notebook markdown cell:

```text
# BIG heading

## Big heading

### SMALL heading

#### small heading
```

Q02.11 Recreate the following table in one Jupyter notebook markdown cell:

| Python Package | Use |
| --- | --- |
| Jupyter | Jupyter notebooks |
| NumPy | arrays |
| Matplotlib | plots |
| PySerial | serial communication |

Q02.12 Recreate the following code block in one Jupyter notebook markdown cell:

```text
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```

Q02.12 Recreate the following bullet points in one Jupyter notebook markdown cell:

 * markdown cell : markdown
 * code cell: Python code
 * raw NBConvert: LaTeX

Q02.13 Recreate the following list in one Jupyter notebook markdown cell:

 1. Open Jupyter notebook
 2. Write code
 3. Restart Kernel & run all
 4. Download notebook
 
Q02.14 Recreate two horizontal rules in a Jupyter notebook markdown cell. In between the horizontal rules write the text _In between the lines_ like below:

***

_In between the lines_

***

Q02.15 Inside a Jupyter notebook markdown cell, make the word ```Red``` the color red, make the word ```Green```, the color green, make the word ```Blue``` the color blue.

Q02.16 Create a warning box on the inside of a Jupyter notebook markdown cell that says: 

**Warning!** Python counting starts at 0 and ends at n-1 

+++

#### LaTeX Math

Q02.20 Write the Pythagorean Theorem in a Jupyter notebook markdown cell using LaTeX math.

$$ a^2 + b^2 = c^2 $$

Q02.21 Write the formula for the area of a circle in a Jupyter notebook markdown cell using LaTeX math.

$$ A = \pi r^2 $$

Q02.22 Write the formula below in a Jupyter notebook Markdown cell using LaTeX math.

$$ \int_{0}^{1} \frac{1}{y^3} dy $$

+++ {"latex": {"environment": "problems"}}

#### Code cells

Q02.31 Run the following code in a Jupyter notebook code cell:

```text
import this
```

Q02.32 Run the following code in a Jupyter notebook code cell:

```text
import sys
print(sys.version)
```

Q02.33 Run the following code in a Jupyter notebook code cell:

```text
import matplotlib.pyplot as plt
%matplotlib inline

plt.plot([1,3,6,10])
plt.show()
```


Q02.34 Run the following code in a Jupyter notebook code cell. Move the slider back and forth and observe the results.

```text
from ipywidgets import interact
import ipywidgets as widgets

def func(x):
    return x
    
interact(func, x=10);
```

+++

#### Cell Magic

Q02.50 Create a file called **_hello.py_** in the same directory as your Jupyter notebook. Inside the file **_hello.py_** write the code below:

```text
# hello.py

print("hello from the file")
```

Use the Jupyter notebook magic command ```%load``` to load the code from **_hello.py_** into your Jupyter notebook.

Q02.51 Create a file called **_hello.py_** in the same directory as your Jupyter notebook. Inside the file **_hello.py_** write the code below:

```text
# hello.py

print("hello from the file")
```

Use the Jupyter notebook magic command ```%run``` to run the code from **_hello.py_** into your Jupyter notebook.

Q02.52 Run the code below in a Jupyter notebook code cell:

```text
import os

print(os.getcwd())

%pwd
```

Why is the output of these two commands similar?

+++

#### Getting Help

Q02.60 Use Python's ```dir()``` function in a Jupyter notebook code cell to find all the functions available in Python's ```math``` module. Remember to ```import math``` at the start of the code cell.

Q02.61 In a Jupyter notebook code cell, ```import math``` and run ```math.sqrt?```. Copy the contents of the help you receive in a Jupyter notebook markdown cell.

Q02.62 In a Jupyter notebook code cell, ```import statistics``` and run ```statistics.mode?```. Copy the examples from the help you receive in a Jupyter notebook code cell. Run the code cell.

```{code-cell} ipython3

```
