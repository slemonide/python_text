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

## Boolean Data Type

+++

The _boolean_ data type is either True or False. In Python, boolean variables are defined by the ```True``` and ```False``` keywords. 

```python
>>> a = True
>>> type(a)
<class 'bool'>

>>> b = False
>>> type(b)
<class 'bool'>
```

The output ```<class 'bool'>``` indicates the variable is a boolean data type.

Note the keywords ```True``` and ```False``` must have an Upper Case first letter. Using a lowercase ```true``` returns an error.

```python
>>> c = true
Traceback (most recent call last):
  File "<input>", line 1, in <module>
NameError: name 'true' is not defined
   
>>> d = false
Traceback (most recent call last):
  File "<input>", line 1, in <module>
NameError: name 'false' is not defined
```

+++

### Integers and Floats as Booleans

Integers and floating point numbers can be converted to the boolean data type using Python's ```bool()``` function. An int, float or complex number set to zero returns ```False```. An integer, float or complex number set to any other number, positive or negative, returns ```True```.

```python
>>> zero_int = 0
>>> bool(zero_int)
False
```

```python
>>> pos_int = 1
>>> bool(pos_int)
True
```

```python
>>> neg_flt = -5.1
>>> bool(neg_flt)
True
```

+++

### Boolean Arithmetic

_Boolean arithmetic_ is the arithmetic of true and false logic. A boolean or logical value can either be ```True``` or ```False```.  Boolean values can be manipulated and combined with _boolean operators_. Boolean operators in Python include ```and```, ```or```, and ```not```.

The common boolean operators in Python are below:

 * ```or```
 * ```and```
 * ```not```
 * ```==``` (equivalent)
 * ```!=``` (not equivalent)

In the code section below, two variables are assigned the boolean values ```True``` and ```False```. Then these boolean values are combined and manipulated with boolean operators.


```python
>>> A = True
>>> B = False
```

```python
>>> A or B
True
```

```python
>>> A and B
False
```

```python
>>> not A
False
```

```python
>>> not B
True
```

```python
>>> A == B
False
```

```python
>>> A != B
True
```

Boolean operators such as ```and```, ```or```, and ```not``` can be combined with parenthesis to make compound _boolean expressions_. 

```python
>>> C = False
>>> A or (C and B)
True
>>> (A and B) or C
False
```

+++

A summary of boolean arithmetic and boolean operators is shown in the table below:

| A | B | not A | not B | A == B | A =! B | A or B | A and B |
| --- | --- | --- | --- | --- | --- | --- | --- |
| T   |   F |   F |   T |   F |   T |   T |   F |
| F   |   T |   T |   F |   F |   T |   T |   F |
| T   |   T |   F |   F |   T |   F |   T |   T |
| F   |   F |   T |   T |   T |   F |   F |   F |

```{code-cell} ipython3

```
