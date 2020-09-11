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

## Print Statements

+++

One built-in function in Python is ```print()```. The value or expression inside of the parenthesis of a ```print()``` function "prints" out to the REPL when the ```print()``` function is called. 

An example using the ```print()``` function is below:

```python
>>> name = "Gabby"
>>> print("Your name is: ")
Your name is: 
>>> print(name)
Gabby
```

Remember that strings must be enclosed by quotation marks. The following command produces an error.

```python
>>> print(Gabby)

NameError: name 'Gabby' is not defined
```

This error is corrected by surrounding the string ```Gabby``` with quotation marks.

```python
>>> print("Gabby")
Gabby
```

+++

Expressions passed to the ```print()``` function are evaluated before they are printed out. For instance, the sum of two numbers can be shown with the ```print()``` function.

```python
>>> print(1+2)
3
```

If you want to see the text ```1+2```, you need to define ```"1+2"``` as a string and print out the string ```"1+2"``` instead.

```python
>>> print("1+2")
1+2
```

+++

Strings can be concatenated (combined) inside of a ```print()``` statement.

```python
>>> name = Gabby
>>> print('Your name is: ' + name)
Your name is Gabby
```

+++

The ```print()``` function also prints out individual expressions one after another with a space in between when the expressions are placed inside the ```print()``` function and separated by a comma.

```python
>>> print("Name:","Gabby","Age", 2+7)
Name: Gabby Age 9
```

```{code-cell} ipython3

```
