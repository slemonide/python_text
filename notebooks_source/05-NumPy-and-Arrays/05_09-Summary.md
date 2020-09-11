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

In this chapter, you learned how to work with NumPy arrays. NumPy is a Python package used for numerical calculations and arrays. An array is a data structure which only contains objects that share the same data type. Arrays are faster than lists in large-scale numerical calculations. 

You learned how to create arrays in a variety of ways:

 * Create an array from a Python list with ```np.array()```
 * Create an array of regularly spaced numbers with ```np.arange()```, ```np.linspace()```, and ```np.logspace```
 * Create an array of random numbers with ```np.random.ranint()```, ```np.random.rand()```, and ```np.random.randn()```
 * Create two 2D arrays from two 1D arrays with ```np.meshgrid()``` and ```np.mgrid()```

You learned how to index and slice arrays. Slicing NumPy arrays share the same syntax used to slice Python lists and strings.

At the end of the chapter, you learned how to run mathematical operations on arrays. NumPy's mathematical functions operate on arrays like Python's math functions operate on integers and floats. NumPy has additional functions like ```np.dot()``` and ```np.cross()``` that cannot be applied to scalars. NumPy's ```np.linalg.solve()``` function can be used to solve systems of linear equations.

+++

### Key Terms and Concepts

+++ {"latex": {"environment": "key_terms"}}

NumPy

array

scalar

computationally expensive

slice

index

data type

homogenous

homogenous data type

element-wise

system of linear equations

attribute

scientific computing

Unicode

iterable

logarithmically spaced numbers

normal distribution

meshgrid

matrix multiplication methods

dot product

cross product

```{code-cell} ipython3

```
