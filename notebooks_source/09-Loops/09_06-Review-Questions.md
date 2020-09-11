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

#### For Loops

+++ {"latex": {"environment": "problems"}}

Q09.01 Create a for loops to print out the numbers 1 to 10.

Q09.02 Create a for loop to print out the number -1 to -10 starting at -1 and ending at -10.

Q09.03 Create a for loop to print out all the letters in the word ```'love'```

Q09.04 Use a for loop to sum the elements in the list ```[1,3,5,8,12]```. Print the sum to the user.

Q09.05 The first 10 terms of the Fibonacci sequence are below:

$$ 1, \ 1, \ 2, \ 3, \ 5, \ 8, \ 13, \ 21, \ 34, \ 55 \ ... $$

Create the Fibonacci sequence using a for loop. Print out the first 20 terms of the Fibonacci sequence on one line. 

Q09.06 This problem is about _Fizz Buzz_, a programming task that is sometimes used in interviews.

(a) Use a for loop to print out the numbers 1 to 30

(b) Use a for loop to print out all the numbers 1 to 30, but leave out any number which is divisible by 3, such as 3, 6 and 9.

(c) Use a for loop to print out all the numbers 1 to 30, but leave out any number which is divisible by 5, such as 5, 10 and 15.

(d) Use a for loop to print out all the numbers 1 to 30, but insert the word ```fizz``` for any number that is divisible by 3, insert the word ```buzz``` for any number that is divisible by 5 and insert the word ```fizz buzz``` for any numbers that are both divisible by 3 and 5, like 15.

Q09.07 Imagine you can see the future of investing and over the next four years, the interest rate of return on investments is going to be 0.02, 0.03, 0.015, 0.06. Prompt the user for an initial investment with Python's ```input(_)``` function and use the formula below to calculate how much the investment will be worth after four years.

new balance = old balance + old balance $\times$ interest rate

Note the first "old balance" is the person's initial investment.

Q09.08 A geometric series is a series that has a common ratio between the terms. The sum of the geometric series that starts at $\frac{1}{2}$ and has a common ratio of $\frac{1}{2}$ approaches the value 1. 

The formula that shows the sum of a geometric series which approaches 1 is below.

$$ 1 = \frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \frac{1}{16} + ... $$

Use the geometric series above to approximate the value of 1 after 10 terms are added. Print out how far off the geometric series approximation is to 1.

Q09.09 A Taylor Series is an infinite series of mathematical terms when summed together approximate a mathematical function. A Taylor Series can be used to approximate the mathematical functions $e^x$, $sine$, and $cosine$.

Taylor Series expansion for the function  $e^x$ is below:

$$  {e^x} = \sum\limits_{n = 0}^\infty  {\frac{{{x^n}}}{{n!}}}  = 1 + x + \frac{{{x^2}}}{{2!}} + \frac{{{x^3}}}{{3!}} + \frac{{{x^4}}}{{4!}} + ... $$

Write a program that asks a user for a number $x$, then calculates $e^x$ using the Taylor Series expansion. Calculate 20 terms.

Q09.10 Write a function called ```lt100()``` that accepts 1 variable as input: a 1D NumPy array.  
The output of ```lt100()``` will be a single 1D NumPy array.

Use a for loop to go through the input NumPy array 1 element at a time starting with element ```0``` going upward.  If the element's value is less than ```100```, put the element into the output 1D NumPy array.  If a value of ```nan``` (Python's not a number) is encountered, stop adding elements to the output variable, but do not raise an exception.  If ```nan``` appears in the first element, the function should return an empty 1D NumPy array, not the ```None``` object.  

Researching the ```numpy.append()``` function will help.  Use ```np.nan``` for testing your code with a ```nan``` value.

Q09.11 Write a function called ```get_bigger()``` that accepts two 1D NumPy arrays for input: ```A``` and ```B```.  ```A``` and ```B``` will contain the same number of elements.  Use a for loop to iterate through both ```A``` and ```B``` one element at a time. If ```A's``` current element is greater than ```B's```, put ```A's``` element into the output 1D  NumPy array variable ```C```. Otherwise, put the sum of the 2 elements into ```C```.  ```C``` will have the same number of elements as both ```A``` and ```B```.

For example, if ```A``` contains ```[5, -10, 1]``` and ```B``` contains ```[2, -10, 8]```, then ```C``` should contain ```[5, -20, 9]```.

Q09.12 Write a function called ```str_add()``` that accepts 1 variable as its input: a list of strings.  Use a for loop to add the character ```'G'``` to the end of each string in the list.  Return the list of altered strings as the only output.

For example, if the list ```['hello', 'bye']``` was passed into your function, the output should be ```['helloG', 'byeG']```.

Q09.13 Write a loop that prints out your name 20 times. Each time your name is printed, it should be on a new line.

Q09.14 Write a loops that prints out "```around and ```" 20 times. Each time "```around and ```" is printed, it should be on the same line. As in ```around and around and around and around and around ...```.

Q09.15 The Appendix contains a section on ASCII character codes. Use code similar to the code shown in the Appendix to print out the ASCII character code and resulting character for just the letters ```a``` to ```z```, ```A``` to ```Z```, and ```0``` to ```9```.

Q09.16 Use a for loop to print out the days of the week. Print each day of the week on its own line.

Q09.17 Use a for loop to print out the spelling of the word ```mississippi``` with one letter on each line.

Q09.18 An employee starts with an annual salary of 58 thousand dollars. Print out the employees salary each year for five years if the employee receives a 2.5 percent (0.02) raise each year.

Q09.19 The factorial function is the product of integers between 1 and n. The formula for factorial is below:

$$ n! = 1 \times 2 \times 3 \times 4 \times 5 \times \ ... \ \times n $$ 

Write a Python function that contains a for loop to find 5 factorial (5!) and 20 factorial (20!)

Q09.20 Create a for loop that prints out all of the even numbers between 1 and 100.

Q09.21 Use Python's ```input()``` function to ask a user for an integer between 1 and 10. Then use a for loop to print out all of the multiples of that number between 1 and 100. Use your program to print out all of the multiples of 9 between 1 and 100.

Q09.22 The Leibniz approximation for the value of $\pi$ is below.

$$ \frac{\pi}{4} = \frac{1}{1} - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \frac{1}{9} - \ ... $$

Use 15 terms in the Leibniz approximation to calculate the value of $\pi$. Compute the error of the Leibniz approximation with 15 terms compared to Pythons ```math.pi``` function. Hint: $(-1)^i$ will alternate in sign as $i$ steps through integers.

Q09.23 Use a for loop to print two columns on each line.  In each line, give an SI prefix, then show which power the prefix corresponds to. Start with "nano" and "10^-9" and end on "giga" and "10^9". An example of the table is below.

```text
nano     10^-9
micro    10^-6
milli    10^-3
...       ...
mega     10^6
giga     10^9
```

Q09.24 Python's ```bin()``` function converts an integer into its binary representation (a number represented as 1's and 0's). Use the ```bin()``` function to build a table of values from 1 to 10 showing the binary representation of each number. Hint: use ```bin(i)[2:]``` to remove ```0b``` from the output of the ```bin()``` function. An example of the table is below.

```text
0     0
1     1
2     10
3     11
4     100
...   ...
```

Q09.25 Iodine-131 is a radioactive isotope of iodine that has a half-life of about 8 days. This means that after 8 days 100g of iodine-131 will decay to 100g/2 = 50g, and after 16 days, 100g of iodine-131 will decay to (100g/2)/2 = 25g. Use a for loop to calculate the mass of 100g of Iodine-131 left after 1 year of radioactive decay.

Q09.26 Use a for loop to ask a user for five numbers. Use another for loop to print out the largest of the five numbers back to the user.

Q09.27 Use a for loop to ask a user for three exam grades. Print back to the user the average of the three grades.

Q09.28 Use a for loop to ask a user for 10 numbers. Print back the the user the mean, median and mode of the numbers. Hint: Python's ```statistics``` module is part of the Standard Library. ```statistics.mean()```, ```statistics.median()``` and ```statistics.mode()``` are three functions present in the ```statistics``` module.

Q09.29 Write a program that requests a word from a user and then counts the number of vowels in the word. The English vowels are ```a, e, i, o, u, y```. Hint: the code ```'a' in ['a','e','i','o','u','y']``` and ```'a' in 'aeiouy'``` both return ```True```.

+++

#### While Loops

+++

Q09.40 Use a while loop to sum the elements in the list ```[1,3,5,8,12]```. Print the sum to the user. 

Q09.41 Use a while loop to print out the numbers between 1 and 100 that have whole number square roots.

Q08.42 Create a program that prompts a user for test scores. Continue to prompt the user for additional test scores until the user types ```'q'```. When the user types ```'q'```, the program stops asking the user for test scores and prints out the following statistics about the test scores the user entered:

 * mean
 * median
 * standard deviation

Q09.43 Use a while loop to validate user input. Ask the user to enter a value between 0 and 1. Print back to the user "Try again" if the user's input is invalid. Print "Your number works!" when the user enters valid input.

Q09.44 Use a while loop to validate user input. Ask the user to enter a day of the week. Keep asking the user for a day of the week until they enter one. When the user enters a day of the week, print "Yup, it's ```<day of the week>```".

Q09.45 Write a program to play the game higher/lower. Tell the user you have picked a random integer between 1 and 20. 

The code below creates a random integer ```n``` between 1 and 20:

```python
from random import randint
n = (randint(1, 20))
```

(a) Ask the user to enter a number (one time) and tell the user if the random number is higher or lower. Print ```higher``` if the random number is higher than the user's guess, print ```lower``` if the random number is lower than the user's guess. Print ```You guessed it: <random number>``` if the user guesses the random number.

(b) Modify your program so that the program keeps printing ```higher``` or ```lower``` after each guess until the user guesses the random number. When the user guesses the random number print ```You guessed it: <random number>```.
    
(c) Extend your higher/lower game to record the number of guesses the user enters to guess the random number. Then the user guesses the random number print ```You guessed: <random number>``` in ```<number of tries>```.
    
Q09.46 A Taylor Series is an infinite series of mathematical terms that when summed together approximate a mathematical function. A Taylor Series can be used to approximate $e^x$, $sine$, and $cosine$.

Taylor Series expansion for the function  $e^x$ is below:

$$  {e^x} = \sum\limits_{n = 0}^\infty  {\frac{{{x^n}}}{{n!}}}  = 1 + x + \frac{{{x^2}}}{{2!}} + \frac{{{x^3}}}{{3!}} + \frac{{{x^4}}}{{4!}} + ... $$

Write a program that asks a user for a number $x$, then calculates $e^x$ using the Taylor Series expansion. Continue to add terms to the Taylor Series until the result from the Taylor series is less than 0.001 off the value of $e^x$ calculated with Python's ```math.exp()``` function. 

+++

#### Errors, Explanations, and Solutions

Run the following code snippets. Explain the error in your own words. Then rewrite the code snippet to solve the error.

+++


Q09.80

```python
n = [1 2 3]
for n[1] == 2:
    n = n + 1
end
```

Q09.81

```python
while x in [1, 2, 3]:
    print(x)
```

Q09.82

```python
n = 1
while 1 == n
    print('valid')
    n = n +1
```

Q09.83

```python
for i in range(3):
print(i)
```

Q09.84

```python
for i in range(5,1):
    print(i)
```

```{code-cell} ipython3

```
