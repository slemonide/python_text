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

# Review Questions

+++

## Line plots

+++ {"latex": {"environment": "problems"}}

Q06.01 Create a plot of the function $y=\cos(x)$ from $x = -2\pi$ to $2\pi$

Q06.02 Create a plot of the function $y=\frac{1}{2}{e^x}$ from $x = 0$ to $5$

Q06.03 Create a plot of the function $y=\sqrt{2x}$ from $x = 1$ to $10$

Q06.04 Create a plot of the function $y=mx+b$, where $m=-1$ and $b=-4$. Limit the plot to values of $x=-5$ to $5$.

Q06.05 Create a plot of the function $y=ax^2+bx+c$, where $a=1/2$, $b=-1/3$ and $c=4$. Limit the plot to values of $x=-10$ to $10$. 

Q06.06 Create a plot of the function $y=x^3+3$ from $x=-3$ to $3$.

Q06.07 Create a plot of the function $y=2x^3-9x^2+7x+6$ from $x=-3$ to $4$.

Q06.08 Plot the data set below with a line plot. Use Matplotlib's default index system, or create a set of x values from $x=0$ to $4$.

$$ y = [-1,\ 2,\ -3,\ 1,\ 0] $$

Q06.09 Plot the following three functions on the same set of axis. Use a different color line for each function.

$$ x = \cos(t) $$

$$ y = \cos(t/2) $$

$$ z = \frac{1}{2}\cos(t) $$

Set values of $t=-4\pi$ to $4\pi$

Q06.10 Plot the following three functions on the same set of axis. Specify a thick red line for the $cos$ function, a thin blue line for the $sin$ function, and a dashed green line for the $atan$ function (the arc tangent function).

$$ x = cos(r/10) $$

$$ y = sin(r/4) $$

$$ z = atan(r) $$

Set values of $r=-1/2$ to $1/2$

+++

### Bar Charts and Pie Charts

+++ {"latex": {"environment": "problems"}}

Q06.30 According to the University of Waterloo, world energy consumption in 2006 from the five top energy resources were:

$$ Natural \ Gas = 24\% $$

$$ Hydro = 6\% $$

$$ Nuclear = 6\% $$

$$ Oil = 36\% $$

$$ Coal = 28\% $$

Build a pie chart of the distribution of world energy consumption based on the data above.

Q06.31 According to the 2017 Python Developer's Survey, the computer operating system used by Python Developers breaks down as follows:

$$ Windows = 49\% $$

$$ Linux = 19\% $$

$$ MacOS = 15\% $$

$$ Other = 17\% $$

Build a pie chart of the computer operating system used by Python Developers in 2017.

Q06.32 According to the 2017 Python Developer's Survey, the commercial cloud providers used by Python Developers breaks down as follows:

$$ Amazon \ Web \ Services = 67\% $$

$$ Google \ Cloud = 29\% $$

$$ Heroku = 26\% $$

$$ Digital \ Ocean = 23\% $$

$$ Microsoft \ Azure = 16\% $$

$$ Other = 13\% $$

Build a pie chart of the commercial cloud providers used by Python Developers in 2017.

Q06.33 Re-create the pie chart in Q06.32 that shows which commercial cloud providers are used by Python Developers. Explode out the pie pieces on the chart and add a shadow to each piece.

Q06.34 Re-create the pie chart in Q06.31 that shows which operating system Python developers use. Explode out the Windows (49%) pie piece to highlight it.

Q06.35 A list of grades in a college engineering course and the corresponding number of students who earned each grade is shown below:

```text
grades = ['A','B','C','D','F']

number_of_students = [3, 5, 8, 1, 2]
```

Build a bar plot of the grade distribution from the college engineering class. 

Q06.36 The proof strength of four different grades of bolts is shown below:

| Bolt Type | Proof Strength (psi) |
| --- | --- |
| Grade 2 | 33,000 psi |
| Grade 5 | 74,000 psi |
| Grade 8 | 120,000 psi |
| Grade A325 | 85,000 psi |

Build a bar chart of the proof strength of the four types of bolts. Label the bars by bolt type and include a title and y-axis label with units.

Q06.37 According to the 2017 Python Developer's Survey, the IDE (Integrated Development Environment) used by _Scientific_ Python Developers breaks down as follows:

$$ PyCharm \ Professional = 12\% $$

$$ PyCharm \ CE = 17\% $$

$$ Sublime \ Text = 9\% $$

$$ Vim = 8\% $$

$$ IDLE = 7\% $$

$$ Atom = 7\% $$

$$ VS \ Code = 6\% $$

$$ Notepad \ ++ = 6\% $$

$$ Eclipse = 3\% $$

$$ Emacs = 3\% $$

Build a bar chart of the IDE's used by Python Developers in 2017.

Q06.38 Create a plot of the function $y=x^3+3$ from $x=-3$ to $x=3$.

Q06.39 The tensile strength of 4 steel heat treatments is shown in the table below:

| Heat Treatment | Tensile Strength (MPa) |
| --- | --- |
| Annealed | 390 MPa |
| Normalized | 452 MPa |
| Oil Quench | 734 MPa
| Oil Quench and Temper | 422 MPa |

Build a bar plot of tensile strength vs. heat treatment using the steel heat treatment data above. Label the bars with the type of heat treatment and include a y-axis label with units and a title.

+++

### Histograms, Box Plots, and Violin Plots

Q06.50 Plot the histogram of a normal distribution of ```100``` random numbers. Use NumPy's ```np.random.normal()``` function to create the array of numbers. Set a mean $\mu$ = ```20``` and a standard deviation $\sigma$ = ```7```.

Q06.51 NumPy's ```np.random.randint()``` function creates an array of random numbers. NumPy's ```np.random.randn()``` function creates an array of normally-distributed random numbers. Use both of these functions to create a set of 200 random numbers. Plot both sets of numbers as histograms with Matplotlib's ```ax.hist()``` method. After you construct both histograms, explain how the two NumPy functions ```np.random.randint()``` and ```np.random.randn()``` compare.

Q06.52 Create a box plot with three elements (three "boxes"). Use NumPy's ```np.random.randn()``` function to create three arrays of 50 elements. Plot each array as a separate element on the box plot.

Q06.53 Create a violin plot with five elements (five "violins"). Use NumPy's ```np.random.randn()``` function to create five arrays of 50 elements. Plot each array as a separate element on the violin plot.

Q06.54 Use Matplotlib's ```plt.subplots()``` command to create a figure with three subplots. In the first subplot, build a historgram. In the second subplot build a box plot. In the third subplot build a violin plot. Plot the same set of 100 normally-distributed random numbers (using NumPy's ```np.random.randn()``` function) in each subplot. Include a title above each subplot that shows the plot type: Histogram, Box Plot, and Violin Plot.

+++

### Scatter Plots

Q06.60 Create a scatter plot with the following lists of x points and y points.

```text
x = [1,2,3,4,5]
y = [8,12,4,2,6]
```

Q06.61 Create a scatter plot with the following arrays of x pints and y points generated with NumPy's ```np.random.randint()``` function.

```text
x = np.random.randint(20)
y = np.random.randint(20)
```

Q06.62 Use the code below to create two arrays of semi-focused random points.

```python
x1 = 1.5 * np.random.randn(150) + 10
y1 = 1.5 * np.random.randn(150) + 10
x2 = 1.5 * np.random.randn(150) + 4
y2 = 1.5 * np.random.randn(150) + 4
x = np.append(x1,x2)
y = np.append(y1,y2)
```

Plot the arrays ```x``` and ```y``` on a scatter plot. Set the color of the marker's on the scatter plot red. Set the marker opacity to ```0.5```.

+++

### Subplots

Q06.70 Create a figure that has four subplots all in one row. In each of the subplots plot the function:

$$ y = e^x $$

Use the same values of x and y in each subplot. Set the values of x with NumPy's ```arange()``` function with the line ```x = np.arange(0.01, 20.0, 0.01)``` In the first subplot, use Matplotlibs's ```ax.plot()``` method. In the second subplot use Matplotlib's ```ax.semilogy()``` method. In the thrid subplot use Matplotlib's ```ax.semilogx()``` method. In the four subplot use Matplotlib's ```ax.loglog()``` method. Label each subplot with a title that shows the plot type.

Q06.71 Use the data in Q06.31 to create a figure with two subplots. In the first subplot, build a bar chart of the data in Q06.31. In the second subplot, build a pie chart of he data in Q06.31.
