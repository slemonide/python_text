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

Q08.01 Create a program to ask a user for a temperature. If the temperature the user enters is below ```50```, print back the user "It is cold outside". Hint: remember to convert the user's input to a number before comparing the user's input to ```50```.

Q08.02 Create a program that asks the user for their temperature. If the user enters a temperature above ```98.6```, print back to the user "You have a fever".

Q08.03 Create a program that chooses a random number number between 1 and 5. Ask the user for a number between 1 and 5. Compare the user's number to the random number. If the user guessed the random number print "you guessed it!", if the user did not guess the random number print back to the user "try again". You can use the code below to choose a random number ```n``` between 1 and 5.

```python
import random

n = random.randint(0,5)
```

Q08.04 Create a program that asks a user for two numbers, x and y. If the x is greater than y, print back to the user "x>y". If x is less than y, print back to the user "x<y". If x is equal to y, print back to the user "x=y".

Q08.05 Create a program that asks a user for one of three trig functions: sine, cosine or tangent. Calculate the sine, cosine or tangent of $\pi/4$ depending on the user's input and print the result of the calculation back to the user.

Q08.06 Create a program that asks the user for two numbers (use two different input lines). If the second number the user enters is zero, print back to the user "can't divide by zero", otherwise divide the user's first number by the user's second number and print the result to the user.

Q08.07 The table below shows a couple fruits and their associated color

| fruit | color |
| --- | --- |
| banana | yellow |
| apple | red |
| lemon | yellow |
| lime | green |
| orange | orange |

Create a program that asks a user to choose from a list of fruit. Print back to the user the color of the fruit they chose.

Q08.08 The average size of a US congressional district is about 700,000 people. Ask the user for a state population and print back to the user the number of congress members in the state. For example, a state with 1.4 million people is represented by 2 members of congress. Each state has at least one member of congress by default. If the user enters a population less than ```700,000```, tell the user their state only has 1 member of congress.

Q08.09 In a college engineering class, final grades are related to percentages as follows:

| percentage range | grade |
| --- | --- |
| 90 - 100 | A |
| 80 - 89 | B |
| 70 - 79 | C |
| 65 - 69 | D |
| 0 - 64 | F |

Build a program that asks a user for a final score (in percent) and prints back to the user their letter grade.

Q08.10 Write a function called ```r()``` that takes in a single variable ```x``` (a numeric value) and outputs a single variable ```y``` (a numeric value). ```y``` should be ```1``` of ```3``` values ```(1, 2, or 3)``` depending on which range ```x``` is in.

range 1: ```x``` is less than ```-10```

range 2: ```x``` is equal to or greater than ```-10``` and less than ```200```

range 3: ```x``` is ```200``` or greater

+++

#### Errors, Explanations, and Solutions

Run the following code snippets. Explain the error in your own words. Then rewrite the code snippet and run the code error-free.

+++


Q08.80

```python
a = 1
if a = 0:
    print('zero')
else if a = 1:
    print('one')
```

+++

Q08.81

```python
a = 1
if a == 0:
    print('zero')
    
else print('one')
```

+++

Q08.82

```python
n = input('Enter a number')

if n > 0:
    print('positive')
```

```{code-cell} ipython3

```
