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

## Flowcharts

+++

Flowcharts graphically represent the flow of a program. There are four basic shapes used in a flow chart. Each shape has a specific use:

 * oval: start / end
 * parallelogram: input / output
 * rectangle: calculations
 * diamond: selection structures
 
![Four basic flow chart shapes: oval, parallelogram, rectangle and diamond](images/four_flow_chart_shapes.png)
 
 Arrows connect the basic shapes in a flowchart. The shapes and arrows of a flowchart describe the flow of a program from start to end. Flowcharts typically flow from the top to the bottom or flow from the left to the right.

+++

Below is the description of a simple program:

 > The program starts. Then the program prints out "Output!". Finally, the program ends.

A flowchart that describes this simple program is shown.

![Flow chart of a simple print program](images/flow_chart_simple_print_program.png)

The Python code that corresponds to this flowchart is:

```python
# start
print("Output!")
# end
```

+++

A description of a program that includes a calculation is below:

 > The program starts. Next, the program asks a user for a number. Two is added to the number. Next, the resulting sum is printed. Finally, the program ends.

A flowchart that describes this program is is shown.

![Flowchart of a program that includes input, output and a calculation](images/flow_chart_calculation_program.png)

The Python code that corresponds to this flow chart is:

```python
# start
num = input("Enter a number: ")
num = float(num)
num_plus_2 = num + 2
print(num_plus_2)
# end
```

+++

The description of another program is below:

 > The program starts. Next the program asks a user for a number. If the number is greater than zero, the program prints "Greater than 0", then the program ends.

A flow chart that describes this program is shown.

![Flow chart of a program that contains user input and a selection structure](images/flow_chart_simple_user_input_program.png)

The Python code that corresponds to this flow chart is:

```python
# start
num = input("Enter a number: ")
num = float(num)
if num>0:
    print("Greater than 0")
# end
```

+++

The description of a more complex program is below:

 > The program starts. Next, the program asks a user for a number. If the number is greater than zero, the program prints "Greater than 0". If the number is less than zero, the program prints "Less than 0". Then the program prints "Done" and the program ends.

A flowchart that describes this program is below:

![Flowchart of a program that contains user input and two if-statements](images/flow_chart_more_complex_user_input_program.png)

The Python code that corresponds to this flow chart is:

```python
# start
num = input('Enter a number: ')
num = float(num)
if num>0:
    print('num greater than zero')
if num<0:
    print('num less than zero')
print('Done')
# end
```

```{code-cell} ipython3

```
