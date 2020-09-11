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

## SymPy

+++

SymPy [http://www.sympy.org](http://www.sympy.org) is a Python library for _symbolic math_.  

In symbolic math, symbols are used to represent mathematical expressions. An example of a symbolic math expression is below.

$$ x^{2} + y^{2} = z $$

The expression contains the symbols $x$, $y$, and $z$.

If we define a second symbolic math expression:

$$ x = a + b $$

then we can substitue in $a + b$ for $x$.

The result is the expression:

$$ (a + b)^{2} + y^{2} = z $$

$$ a^{2} + 2ab + b^{2} + y^{2} = z $$

Solving for $y$ in terms of $a$, $b$ and $z$ results in:
    
$$ y = \sqrt{z - a^{2} - 2ab - b^{2}} $$

In the symbolic math substitution above, symbolic math variables were rearranged, grouped and inserted. None of the variables were equal to a specific number, like 5 or 0.001, but we can still solve for one variable in terms of the other variables when we use symbolic math.

+++

If we have numerical values for $z$, $a$ and $b$, we can use Python to calculate the value of $y$. 

But if we don't have numerical values for $z$, $a$ and $b$, Python and the SymPy package can be used to rearrange terms and solve for one variable in terms of the other.

Working with mathematical symbols in a programmatic way instead of working with numerical values in a programmatic way is called _symbolic math_.
