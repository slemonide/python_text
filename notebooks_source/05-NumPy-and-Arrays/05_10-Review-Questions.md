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

+++

#### Array Creation

+++ {"latex": {"environment": "problems"}}

Q05.01 Create an array of the numbers ```1```, ```5```, ```19```, ```30```

Q05.02 Create an array of the numbers ```-3```, ```15```,```0.001```, ```6.02e23```

Q05.03 Create an array of integers between -10 and 10

Q05.04 Create an array of 10 equally spaced angles between 0 and 2$\pi$

Q05.05 Create an array of logarithmically spaced numbers between 1 and 1 million. Hint: remember to pass exponents to the ```np.logspace()``` function.

Q05.06 Create an array of 20 random integers between 1 and 10

Q05.07 Create an array of 30 random numbers with a normal distribution

Q05.08 Create an array of 30 random numbers with a normal distribution that has an mean $\mu$ of 78.5 and a standard deviation $\sigma$ of 5.2

Q05.09 Create an array of 18 random floating point numbers between 0 and 1

Q05.10 Create an array of 18 random floating point numbers between -1 and 0

Q05.11 Create an array of 18 random floating point numbers between 0 and 10

Q05.12 Create a variable $x$ that is an NumPy array which contains values 0, 0.1, 0.2, ..., 4.9, 5.0.  Hard coding the values one will be time consuming, use a NumPy function to create the array instead.

Q05.13 Create a Python list containing the values 1, 2, 5.6, and 9 and store the Python list in a variable called ```x```.  Then create a NumPy array of the same values and store it in a variable called ```y```.

Q05.14 Create an array called ```r``` of 200 evenly spaced numbers between and including 0 to 2$\pi$, then create an array ```y``` such that $y=10sin(3r)$.

Q05.15 Create an array of 25 regularly spaced values beginning at 10 and ending with 18.

Q05.16 Create an array of regularly spaced numbers beginning at 10, ending with 18.4 using an increment of 0.6.

+++

#### Array Manipulation

+++

Q05.20 Create a NumPy array called ```A``` and store the values 5, 8, -8, 99, and 0 in array ```A``` in a single row, five columns. Reshape ```A``` to an array with one column and 5 rows.

+++

#### Array Slicing

+++

Q05.30 Create an array ```B``` that contains integers 0 to 24 (including 24) in one row.  Then reshape ```B``` into a 5 row by 5 column array.

(a) Extract the 2nd row from ```B```.  Store it as a one column array called ```x```.

(b) Store the number of elements in array ```x``` in a new variable called ```y```. 

(c) Extract the last column of ```B``` and store it in an array called ```z```.  

(d) Store a transposed version of ```B``` in an array called ```t```.

Q05.31 Run the following code to create a NumPy array ```C```

```C = np.array(range(11)) + 5```

(a) Extract the 4th value in array ```C``` into a variable called ```x```.

(b) Extract the 2nd-to-last value in array ```C``` into a variable called ```y```.

(c) Extract the values from array ```C``` starting from the 3rd value up to and including the 7th value into a variable called ```z```.

Q05.32 Run the following code to create a NumPy array ```D```

```D = np.array(range(18)) + 3```

(a) Extract every other value from array ```D``` starting from the 2nd value through the 10th value.  Store the result in a variable called ```x```.

(b) Extract every other value from array ```D``` starting from the 10th value through the 2nd value.  Store the result a variable called ```y```.

(c) Create a variable ```z``` that contains all of the values in ```D``` in reverse order.

Q05.33 The 1D NumPy array ```F``` is defined below.  But construct your code to work with any 1D NumPy array filled with numbers.

```F = np.array([5, -4.7, 99, 50, 6, -1, 0, 50, -78, 27, 10])```

(a) Select all the elements from ```F``` that are greater than ```5``` and store them in ```x```.

(b) Select all of the elements from ```F``` that are between ```5``` and ```30```.  Store them in ```y```.

(c) Select all of the elements from ```F``` that are between ```5``` and ```30``` or that are equal to ```50```.  Store them in ```z```.

Hint: To perform the logical ```OR``` or ```AND``` operations, on boolean arrays of the same dimensions, NumPy functions are needed.  The standard Python ```"or"``` and ```"and"``` will not work. 

Hint: You can use either logical indexing or ```np.where()``` to get the appropriate values from ```A```.

Q05.34 The 1D NumPy array ```B``` is defined below.  But your code should work with any 1D NumPy array filled with numeric values.

```G = np.array([5, -4.7, 99, 50, 6, -1, 0, 50, -78, 27, 10])```

(a) Select all of the positive numbers in ```G``` and store them in ```x```.

(b) Select all the numbers in ```G``` between ```0``` and  ```30``` and store them in ```y```.

(c) Select all of the numbers in ```G``` that are either less than ```-50``` or greater than ```50``` and store them in ```z```.

Q05.35 Define an integer ```c``` which is a random integer between ```100``` and ```999``` (including ```100``` and ```999```)

(a) pull the first digit out of ```c``` and assign it to the variable ```x```

(b) pull the second digit out of ```c``` and assign it to the variable ```y```

(c) pull the third digit out of ```c``` and assign it the the variable ```z```.

+++

#### Meshgrids

+++

Q05.40 Create two 2D arrays from the two 1D arrays below using NumPy's ```np.meshgrid()``` function. 

```text

x = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5]

y = [0, 2, 4, 6]
```

Q05.41 Create a meshgrid of the two arrays below:

```text

x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

y = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

Use element-wise multiplication to multiply each element in the first resulting 2D array with the corresponding element is the second array to build a multiplication table.

+++

#### Array Operations

Q05.50 Create the two arrays below and perform each calculation.

```a = [2 4 6]```

```b = [-1 0 1]```

(a) $a + b$

(b) $1.5a -2b$

(c) $0.5ab$

(d) $\frac{b^2}{a}$


Q05.51 Create an array of angles between (and including) 0 and 2$\pi$ radians in increments of $\pi/2$ radians.

(a) Calculate the sine of each angle in the array

(b) Calculate the cosine of each angle in the array

(c) Convert each angle in the array to degrees

Q05.52 Create the two arrays ```F1```, ```F2``` below and then perform the following operations.

```F1 = [-1, 0, 2]```

```F2 = [5, -2, 0]```

(a) Calculate the dot product of ```F1``` and ```F2```

(b) Calculate cross product of ```F1``` and ```F2```

(c) Calculate the element-wise product (element-wise multiplication of ```F1``` and ```F2```)

Q05.53 Compute all possible prices of flooring that can have lengths of ```2```, ```4```, ```6```, and ```8``` meters and widths of ```1```, ```1.5```, and ```2``` meters if the flooring costs \$32.19 per square meter. Store the result in a 2D array. The lengths should increase from top to bottom and widths should increase from left to right.

Q05.54 Create an array ```H``` defined by the code below:

```H = np.array([-5, 10, 12, 500, 20, 10, -46, 16])```

(a) Create a boolean array ```x``` based on the variable ```H```.  ```x``` should be ```True``` everywhere ```H``` equals ```10``` and ```False``` everywhere else.

(b) Create a boolean array ```y``` based on the variable ```H```.  ```y``` should be ```True``` everywhere ```H``` is not equal to ```10```.  ```y``` should be ```False``` everywhere else.

(c) Create a boolean array ```z``` based on the variable ```H```.  ```z``` should be ```True``` everywhere ```H``` is less than or equal to ```20```.  ```z``` should be ```False``` everywhere else.

Q05.55 Create an array ```J``` using the code below:

```
J = np.array(range(7*5)).reshape((7, 5))
J[4, 3] = 500
```

(a) Store the row index of the number ```500``` in a variable called ```row_500```.

(b) Store the column index of the number ```500``` in a variable called ```col_500```.

Q05.56 Create an array ```K``` using the code below:

```
K = np.random.randint(100, 500, 7*7).reshape(7, 7)
K[2, 6] = 250
```

(a) Extract all of the values from ```K``` that are greater or equal to ```250```` and store them in an array called ```x```. 

(b) Extract all of the values from ```K``` that are less than ```250``` and store them in an array called ```y```.

(c) Programmatically determine which column and which row the number ```250``` is stored inside of ```K```. 

+++

#### Linear Algebra

+++

Q05.70 Use the system of linear equations below to calculate the values of $x$ and $y$.

$$ 4x - 2y = -42 $$

$$ -6x + y = 31 $$

Q05.71 Use the system of linear equations below to calculate the values of $x$, $y$ and $z$.

$$ \frac{x}{2} +2y - z = 5 $$

$$ x + 3y - 4z = -1 $$

$$ -x - 3y + 2z = -5 $$

```{code-cell} ipython3

```
