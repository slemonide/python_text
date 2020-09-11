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

## Numeric Data Types

+++

Python has many useful built-in _data types_. Python variables can store different types of data based on a variable's data type. A variable's data type is created dynamically, without the need to explicitly define a data type when the variable is created.

It is useful for problem solvers to understand a couple of Python's core data types in order to write well-constructed code. 

+++

### A review of variable assignment in Python

Recall from the previous chapter that variables in Python are defined with the assignment operator, the equals sign ```=```.  To define a variable in Python, the variable name is written first, then the assignment operator ```=``` followed by a value or expression.

The general syntax to assign a value to variable name is below:

```text
variable_name = value
```

Variable names in Python must adhere to the following rules:

 * variable names must start with a letter
 * variable names can only contain letters, numbers and the underscore character ```_```
 * variable names can not contain spaces or punctuation
 * variable names are not enclosed in quotes or brackets


Below is a discussion of a few different built-in data types in Python.

+++

### Integers

_Integers_ are one of the Python data types. An integer is a whole number, negative, positive or zero. In Python, integer variables are defined by assigning a whole number to a variable. Python's ```type()``` function can be used to determine the data type of a variable.

```python
>>> a = 5
>>> type(a)
<class 'int'>
```

The output ```<class 'int'>``` indicates the variable ```a``` is an integer. Integers can be negative or zero.

```python
>>> b = -2
>>> type(b)
<class 'int'>
>>> z = 0
>>> type(z)
<class 'int'>
```

+++

### Floating Point Numbers

Floating point numbers or _floats_ are another Python data type. Floats are decimals, positive, negative and zero. Floats can also be represented by numbers in scientific notation which contain exponents.

Both a lower case ```e``` or an upper case ```E``` can be used to define floats in scientific notation. In Python, a float can be defined using a decimal point ```.``` when a variable is assigned.

```python
>>> c = 6.2
>>> type(c)
<class 'float'>
>>> d = -0.03
>>> type(d)
<class 'float'>
>>> Na = 6.02e23
>>> Na
6.02e+23
>>> type(Na)
<class 'float'>
```

To define a variable as a float instead of an integer, even if the variable is assigned a whole number, a trailing decimal point ```.``` is used. Note the difference when a decimal point ```.``` comes after a whole number:

```python
>>> g = 5
>>> type(g)
<class 'int'>
>>> f = 5.
>>> type(r)
<class 'float'>
```

+++

### Complex Numbers

Another useful numeric data type for problem solvers is the _complex number_ data type. A complex number is defined in Python using a real component ```+``` an imaginary component ```j```. The letter ```j``` must be used to denote the imaginary component. Using the letter ```i``` to define a complex number returns an error in Python.

```python
>>> comp = 4 + 2j
>>> type(comp)
<class 'complex'>

>>> comp2 = 4 + 2i
              ^
SyntaxError: invalid syntax
```

Imaginary numbers can be added to integers and floats.

```python
>>> intgr = 3
>>> type(intgr)
<class 'int'>

>>> comp_sum = comp + intgr
>>> print(comp_sum)
(7+2j)

>>> flt = 2.1
>>> comp_sum = comp + flt
>>> print(comp_sum)
(6.1+2j)
```

```{code-cell} ipython3

```
