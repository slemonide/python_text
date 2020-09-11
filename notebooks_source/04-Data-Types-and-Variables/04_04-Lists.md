---
jupytext:
  cell_metadata_filter: all
  notebook_metadata_filter: all,-language_info,-toc,-latex_envs
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.10'
    jupytext_version: 1.5.2
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

## Lists

+++

A list is a data structure in Python that can contain multiple elements of any of the other data type. A list is defined with square brackets ```[ ]``` and commas ``` , ``` between elements.

```python
>>> lst = [ 1, 2, 3 ]
>>> type(lst)
list

>>> lst = [ 1, 5.3, '3rd_Element']
>>> type(lst)
list
```

+++

### Indexing Lists

Individual elements of a list can be accessed or _indexed_ using bracket ```[ ]``` notation. Note that Python lists start with the index zero, not the index 1. For example:

```python
>>> lst = ['statics', 'strengths', 'dynamics']
>>> lst[0]
'statics'

>>> lst[1]
'strengths'

>>> lst[2]
'dynamics'
```

+++ {"latex": {"environment": "alert-danger"}}

<div class="alert alert-danger">
<strong>Remember!</strong> Python lists start indexing at [0] not at [1]. To call the elements in a list with 3 values use: lst[0], lst[1], lst[2].
</div>

+++

### Slicing Lists

Colons ``` : ``` are used inside the square brackets to denote _all_

```python
>>> lst = [2, 4, 6]
>>> lst[:]
[2, 4, 6]
```

Negative numbers can be used as indexes to call the last number of elements in the list

```python
>>> lst = [2, 4, 6]
>>> lst[-1]
6
```

The colon operator can also be used to denote _all up to_ and _thru end_.

```python
>>> lst = [2, 4, 6]
>>> lst[:2]         # all up to 2
[2, 4]
```


```python
>>> lst = [2, 4, 6]
>>> lst[2:]         # 2 thru end
[6]
```

The colon operator can also be used to denote _start : end + 1_. Note that indexing here in not inclusive. ```lst[1:3]``` returns the 2nd element, and 3rd element but not the fourth even though ```3``` is used in the index.

+++ {"latex": {"environment": "alert-danger"}}

<div class="alert alert-danger">
<strong>Remember!</strong> Python indexing is not inclusive. The last element called in an index will not be returned.
</div>

```{code-cell} ipython3

```
