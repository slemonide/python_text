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

+++ {"latex": {"environment": "problems"}}

#### Determine the Data Type

Q04.01 Find the data type of ```a``` if ```a=9```

Q04.02 Find the data type of ```a``` if ```a=9.```

Q04.03 Find the data type of ```a``` if ```a='9.'```

Q04.04 Find the data type of ```a``` if ```a=(9)```

Q04.05 Find the data type of ```a``` if ```a=False```

Q04.06 Find the data type of ```a``` if ```a=[1,2,3]```

Q04.07 Find the data type of ```a``` if ```a=(1,2,3)```

Q04.08 Find the data type of ```a``` if ```a={'key': 9}```

Q04.09 Find the data type of ```a``` if ```a=1 + 9j```

+++

#### Numeric Data Types

Q04.10 Set ```a=1``` and ```b=2```. What data type is ```a/b```?

Q04.11 Set ```a=1``` and ```b=2```. What data type is ```a*b```?

Q04.12 What is ```5.1``` plus ```0 + 3j```?

Q04.13 What floating point number converts to the boolean ```False```? Show this in code using the ```bool()``` function.

Q04.14 Create the floating point number $0.001 \times 10^{-0.2}$ and assign it to the variable ```b```.

Q04.15 Show that ```3e2``` is the same as ```3E2``` with the comparison operator ```==```

Q04.16 Euler's number, $e$, can be called in Python using the code below:

```
from math import e
```

(a) Round $e$ to the nearest integer. Store the result in a variable called ```x```.

(b) Round $e$ to the nearest 1000ths place (the nearest 0.001). Store the result in a variable called ```y```.

(c) Truncate the decimal portion of $e$ (remove the 0.71828.... portion) so you are left with the integer ```2```. Store the result in a variable called ```z```. Hint: convert $e$ to a string and use string slicing.

Q04.17 Define the complex number ```A``` using the code below:

```A = 4 + 2j```

(a) store the real component of ```A``` in a variable called ```real```.

(b) store the imaginary component of ```A``` in a variable called ```imaginary```.

(c) store the magnitude of ```A``` in a variable called ```mag```. The magnitude of an imaginary number is defined as:

$$ magnitude = \sqrt{(real)^2+(imaginary)^2} $$

+++

#### Booleans

Q04.20 Predict the output if the lines ```n=5``` and ```(n<3) and (n<7)``` are run. Then run the the two lines of code.

Q04.21 Predict the output if the lines of code below are run. Then run the code.

```python
>>> ans='Yes'
>>> ans=='Yes' or ans=='No'
```

Q04.22 Pick a number ```n``` to make the following statement ```True```: ```(2<n) or (n==2+n)``` Then run the code to show your number works.

Q04.23 Pick a number ```n``` to make the following statement ```False```: ```not (n<6) and (n<4)``` Then run the code to show your number works.

Q04.24 Add the integers ```1``` and ```0``` and convert the answer to a boolean. Add the boolean values ```bool(0) + bool(1)``` and compare the result. 

Q04.25 Show that ```(n>5) and (n<=10)``` is equivalent to ```5 < n <= 10``` using the two different numbers for ```n```.

Q04.26 Show that ```(n<5) or (n>=10)``` is equivalent to ```not(5 =< n < 10)``` using the two different numbers for ```n```.

+++

#### Strings

Q04.30 Define a string that contains the word $Problem$.

Q04.31 Define one string as the word $Problem$ and define another string as the word $Solving$. Combine these two strings to make the statement $Problem \ Solving$.

Q04.32 (a) Define a string that contains the number $8$ and a string that contains the number $5$. Combine these two strings with the plus operator ```+```.

 (b) Define an integer as the number $8$ and an integer as the number $5$ and combine these two integers with the plus operator ```+```
 
 (c) Explain why the output from (a) was different from the output of (b)
 
 (d) Multiply the string $8$ and the string $5$ with the multiplication operator ```*```.  Compare the output to multiplying the integers $8$ and the integer $5$. Why is the output different?

Q03.33 Complete the following index and slicing operations after ```word = 'Problem'``` is defined.

(a) Pull out the letter $P$ from ```word```

(b) Pull out the first three letters $Pro$ from ```word```

(c) Pull out the second through the fourth letters $rob$ from ```word```

(d) Pull out every other letter from ```word``` starting with $P$

(e) Use indexing and slicing to ouput ```word``` backwards to produce $melborP$.

Q04.34 Define the strings below:

 (a) Define a string ```a``` as _coffee_,  define a string ```b``` as _it's_, define a string ```c``` as _hot!_ and string ```d``` as , (a comma).
 
 (b) Combine the strings ```a```, ```b```, ```c``` and ```d``` to produce the string _coffee, it's hot_ (notice the comma)
 
 (c) Print out the statement _she said "coffee, it's hot"_ using the variables ```a```, ```b```, ```c``` and ```d```.
 
Q04.35 Create the string ```path``` with the value _C:\\Users\\Gabby\\Documents_

Q04.36 Convert the string ```Problem``` to the list ```['P','r','o','b','l','e','m']``` without writing the list from scratch.

Q04.37 Use the string ```over board``` and slicing to produce the following words:

(a) ```over```

(b) ```board```

(c) ```oar```

Q04.38 Use the string ```rotten tomatoes``` and slicing to produce the following words:

(a) ```to```

(b) ```no```

(c) ```ten```

(d) ```oat```

+++

#### Lists

Q04.40 Create a list that contains the numbers $1$, $2.9 \times 10^8$, and the word $game$.

Q04.41 Create a list that contains the words $problem$, $solving$, $with$, $python$.

Q04.42 Create a list with one value, the number $6$. Convert the list to a boolean with the ```bool()``` function.

Q04.43 Create an empty list. Convert the empty list to a boolean with the ```bool()``` function.

Q04.44 Create a list with the letters $C$, $D$, and $R$. Pull the letters $C$ and $D$ out of your list with indexing.

Q04.45 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to pull out the number $5$ from the list.

Q04.46 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to pull out all of the numbers $5$ or less.

Q04.47 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to pull out all of the numbers $5$ and greater.

Q04.48 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to pull out all of the even numbers from the list.

Q04.49 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to pull out every odd number from the list.

Q04.50 Create a list with the numbers $1$ to $10$ (counting by ones). Use slicing to return the list in reverse order (the returned list starts with $10$ and ends with $1$).

Q04.51 Create a Python list containing the values 1, 2, 5.6, and 9 in that order and store it in a variable called ```x```. 

+++

#### Dictionaries

Q04.60 Create a dictionary called ```capitals``` that contains the states and state capitals. Include ```Washington```, capital ```Olympia``` and ```Oregon```, capital ```Salem```.

Q04.61 Create a dictionary called ```capitals``` that contains the states and state capitals. Include ```Washington```, capital ```Olympia``` and ```Oregon```, capital ```Salem```. In the line after the dictionary is created add the state ```New York```, capital ```Albany```.

Q04.62 Create a dictionary ```numbers = {'one':1, 'two':2, 'three':3}```. Pull out the number ```'2'``` by calling the key ```'two'```.

Q04.63 Create a dictionary ```colors = {'red':'	#FF0000', 'green':'#008000', 'blue':'#0000FF'}```. Pull out all the keys and add them to a list called ```colors_list``` with the ```.keys()``` method.

Q04.64 Create a dictionary ```colors = {'red':'	#FF0000', 'green':'#008000', 'blue':'#0000FF'}```. Pull out all the values and add them to a list called ```colors_hex``` with the ```.values()``` method.

Q04.65 Create a dictionary ```colors = {'red':'	#FF0000', 'green':'#008000', 'blue':'#0000FF'}```. Pull out all the items from the dictionary and add them to a list called ```color_items``` with the ```.items()``` method.

Q04.66 Create a dictionary ```groups = {'solo':1, 'duo':2}```. Add the key ```'trio'``` and the corresponding value ```3```.

Q04.67 Create a dictionary ```groups = {'solo':1, 'duo':2}```. Then remove the key ```'duo'``` and the value ```2``` so that only ```'solo':1``` remains.

Q04.68 Create a dictionary ```college = {'name': 'University of Oregon'}```. Add the following two keys: $abbreviation$, $mascot$ and the corresponding two values: $UofO$, $ducks$.

+++

#### Tuples

Q04.70 Create a tuple with the numbers $8$, $9$, and $10$. 

Q04.71 Create a tuple that has a single entry, the number $10$.

Q04.72 Create a list and a tuple that both contains the strings: $one$, $two$ and $three$.   Pull the word $two$ out of both the list and the tuple.

Q04.73 Create a list and a tuple that both contains the strings: $one$, $two$ and $three$. Try to substitute the number $2$ for the word $two$ in both the list and tuple using indexing (square brackets).

Q04.74 Code the following lines:

```python
t1 = (9)
t2 = (9,)
t3 = ('9')
```

Use Python's ```type()``` function to find the object type of each variable.

Q04.75 Create a tuple that returns ```True``` when converted to a boolean. Use the ```bool()``` function to demonstrate your tuple converts to ```True```.

Q04.76 Create a tuple that returns ```False``` when converted to a boolean. Use the ```bool()``` function to demonstrate your tuple converts to ```False```.

+++ {"latex": {"environment": "problems"}}

#### Errors, Explanations, and Solutions

Q04.80 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
n = 503
n[2]
```

Q04.81 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
a = 321
b = 'go!'
c = a + b
```

Q04.82 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
d = {one:1, two:2, three:3}
d[one]
```

Q04.83 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
f = false
not f
```

Q04.84 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
comp = 0.1 - 4.3i
comp + 5
```

Q04.85 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
empty = ''
bool(empty)
```

Q04.86 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
lst = [1,3,5]
lst[3]
```

Q04.87 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
dict = ['key': 8, 'pair': 9]
dict['key']
```

Q04.88 Run the following lines of code and explain the error in your own words. Then rewrite the lines of code to run error free:

```python
s = ['Problem Solving']
s[8:]
```

```{code-cell} ipython3

```
