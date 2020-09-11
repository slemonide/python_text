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

## Flowcharts Describing Loops

+++

Flowcharts show the flow of a program graphically. Flow charts were introduced in the previous chapter to describe how a programs that include _if_ statements are illustrated graphically.

This chapter is about _loops_. Flowcharts can also be used to describe programs which contain _for loops_ and _while loops_.

+++

### Basic Flow Chart Shapes

+++

Let's review the four basic flowchart shapes. Each shape represents a different type of operation.

 * oval: start and end
 * parallelogram: input and output
 * rectangle: calculations
 * diamond: selection structures
 
![Four the four flowchart shapes: oval, parallelogram, rectangle, and diamond](images/four_flow_chart_shapes.png)
 
The basic shapes in a flowchart are connected by arrows. The shapes and arrows in a flowchart represent the flow of a program from start to end.

+++

### Flowchart of a program that contains a for loop

+++

Below is the description of a program that can be coded with a for loop:

 > The program starts. The program prints the word "looping" 10 times. Finally, the program ends.

A flowchart that describes this program is shown.

![Flowchart of a program that contains a for loop](images/flow_chart_of_program_that_contains_a_for_loop.png)

The Python code that corresponds to this flowchart is below:

```python
# start
for i in range(10):
    print("looping")
# end
```

+++

### Flowchart of a program that contains a while loop

+++

Below is the description of a program which can be coded with a while loop:

 > The program starts. The program asks the user for a positive number. If the number is negative, the program asks the user for a positive number again. If the number is positive, the program prints "positive". Finally, the program ends.

A flowchart that describes this program is shown.

![Flow chart of a program that contains a for loop](images/flow_chart_of_program_that_contains_a_while_loop.png)

The Python code that corresponds to this flow chart is:

```python
# start
num = -1
while num < 0:
    num = input("Enter a positive number: ")
    num = float(num)
print("positive")
# end
```

```{code-cell} ipython3

```
