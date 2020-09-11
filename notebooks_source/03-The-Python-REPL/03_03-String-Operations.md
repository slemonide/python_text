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

## String Operations

+++

Strings are sequences of letters, numbers, punctuation, and spaces. Strings are defined at the Python REPL by enclosing letters, numbers, punctuation, and spaces in single quotes ```' '``` or double quotes ```" "```. 

```python
>>> word = "Solution"
>>> another_word = "another solution"
>>> third_word = "3rd solution!"
```

In Python, string operations include concatenation (combining strings), logical comparisons (comparing strings) and indexing (pulling specific characters out of strings).

+++

### String Concatenation

+++

Strings can be _concatenated_ or combined using the ```+``` operator.

```python
>>> word = "Solution"
>>> another_word = "another solution"
>>> third_word = "3rd solution!"
>>> all_words = word+another_word+third_word
>>> all_words
'Solutionanother solution3rd solution!'
```

To include spaces in the concatenated string, add a string which just contains one space ```" "``` in between each string you combine.

```python
>>> word = "Solution"
>>> another_word = "another solution"
>>> third_word = "3rd solution!"
>>> all_words = word + " " + another_word + " " + third_word
>>> all_words
'Solution another solution 3rd solution!'
```

+++

### String Comparison

+++

Strings can be compared using the comparison operator; the double equals sign ```==```. Note the comparison operator (double equals ```==```) is not the same as the assignment operator, a single equals sign ```=```.

```python
>>> name1 = 'Gabby'
>>> name2 = 'Gabby'
>>> name1 == name2
True
```

```python
>>> name1 = 'Gabby'
>>> name2 = 'Maelle'
>>> name1 == name2
False
```

Capital letters and lower case letters are different characters in Python. A string with the same letters, but different capitalization are not equivalent.

```python
>>> name1 = 'Maelle'
>>> name2 = 'maelle'
>>> name1 == name2
False
```

```{code-cell} ipython3

```
