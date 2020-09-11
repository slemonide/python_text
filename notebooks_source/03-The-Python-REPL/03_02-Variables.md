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

## Variables

+++

Variables are assigned in Python using the ```=``` equals sign also called the _assignment operator_. The statement:

```python
a = 2
```

Assigns the integer ```2``` to the variable ```a```.

+++

```python
>>> a = 2
>>> a
2
```

+++

Note the assignment operator ```=```(equals), is different from the logical comparison operator ```==``` (equivalent to).

+++

```python
>>> a == 2
True
```

+++

Variable names in Python must conform to the following rules:

 * variable names must start with a letter
 * variable names can only contain letters, numbers, and the underscore character ```_```
 * variable names can not contain spaces
 * variable names can not include punctuation
 * variable names are not enclosed in quotes or brackets

+++

The following code lines show valid variable names:

+++

```text
constant = 4

new_variable = 'var'

my2rules = ['rule1','rule2']

SQUARES = 4
```

+++

The following code lines show invalid variable names:

+++

```text
a constant = 4

3newVariables = [1, 2, 3]

&sum = 4 + 4
```

+++

Let's solve the problem below at the Python REPL using variables.

#### Problem

The Arrhenius relationship states:

$$ n = n_{v}e^{-Q_v/(RT)} $$

In a system where $n_v = 2.0 \times 10^{-3}$, $Q_v = 5$, $R=3.18$, and $T=293$, calculate $n$.

#### Solution

Use variables to assign a value to each one of the constants in the problem and calculate $n$.

```python
>>> nv = 2.0e-3
>>> Qv = 5
>>> R = 3.18
>>> T = 293
>>> from math import exp
>>> n = nv*exp(-1*Qv/(R*T))
>>> n
0.0019892961379660424
```

```{code-cell} ipython3

```
