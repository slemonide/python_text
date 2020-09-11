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

## Break and Continue

+++

_Break_ and _continue_ are two ways to modify the behavior of for loops and while loops.

+++

### Break

In Python, the keyword ```break``` causes the program to exit a loop early. ```break``` causes the program to jump out of for loops even if the for loop hasn't run the specified number of times.```break``` causes the program to jump out of while loops even if the logical condition that defines the loop is still ```True```.

An example using ```break``` in a for loop is below.

```{code-cell} ipython3
for i in range(100):
    print(i)
    if i == 3:
        break
print('Loop exited')
```

When the loop hits ```i=3```, ```break``` is encountered and the program exits the loop. 

An example using ```break``` in a while loop is below.

```{code-cell} ipython3
while True:
    out = input('type q to exit the loop: ')
    if out == 'q':
        break
print('Loop exited')
```

### Continue

In Python, the keyword ```continue``` causes the program to stop running code in a loop and start back at the top of the loop. Remember the keyword ```break``` cause the program to _exit_ a loop. ```continue``` is similar, but ```continue``` causes the program to stop the _current iteration_ of the loop and _start the next iteration at the top_ of the loop.

A code section that uses ```continue``` in a for loop is below.

```{code-cell} ipython3
for i in range(4):
    if i==2:
        continue
    print(i)
```

When the code section is run, the number ```2``` is not printed. This is because when ```i=2``` the program hits the  ```continue``` statement. Therefore, the line ```print(i)``` isn't run when ```i=2```. Then the program starts back up at the start of the loop with the next number ```i=3```.
