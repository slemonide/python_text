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

In this chapter, you learned about a couple of different data types built-in to Python. These data types include the numeric data types: integers, floats, and complex numbers. The string data type is composed of letters, numbers, spaces, and punctuation. Python also has container data types which can store many values. These container data types include lists, tuples, and dictionaries. Strings, lists and tuples can be indexed and sliced using square brackets ```[ ]```.

+++

### Key Terms and Concepts

+++ {"latex": {"environment": "key_terms"}}

data type

variable

assignment operator

integer

int

whole number

floating point number

float

scientific notation

complex number

string

boolean

bool

boolean arithmetic

boolean operators

or

and

not

data structure

dictionary

tuple

list

index

indexing

immutable

+++

### Summary of Python Functions and Commands

+++

#### Built-in Data Types

| Python Data Type | Description |
| --- | --- |
| ```int``` | integer |
| ```float``` | floating point number |
| ```bool``` | boolean value: True or False |
| ```complex``` | complex number, real and imaginary components |
| ```str``` | string, sequence of letters, numbers and symbols |
| ```list``` | list, formed with ```[ ]``` |
| ```dict``` | dictionary, formed with ```{'key'=value}``` |
| ```tuple``` | an immutable list, formed with ```( )``` |

#### Python Functions

| Function | Description |
| --- | --- |
| ```type()``` | output a variable or object data type |
| ```len()``` | return the length of a string, list dictionary or tuple |
| ```str()``` | convert a ```float``` or ```int``` into a ```str``` (string) |
| ```int()``` | convert a ```float``` or ```str``` into an ```int``` (integer) |
| ```float()``` | convert an ```int``` or ```str``` into an ```float``` (floating point number) |

#### Python List Operators

| Operator | Description | Example | Result |
| --- | --- | ---- | --- |
| ```[ ]``` | indexing | ```lst[1]``` | ```4``` |
| ```:``` | start | ```lst[:2]``` | ```[ 2, 4 ]``` |
| ```:``` | end | ```lst[2:]``` | ```[ 6, 8 ]``` |
| ```:``` | through | ```lst[0:3]``` | ```[ 2, 4, 6 ]``` |
| ```:``` | start, step, end+1 | ```lst[0:5:2]``` | ```[2, 6]``` |

```{code-cell} ipython3

```
