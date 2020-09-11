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

#### Creating Expressions Equations

+++

Q10.01 Create the symbolic math variables $a$, $b$, $c$ and $x$. Use these variables to define the symbolic math expressions:

$$ ax^2 + bx + c $$

$$ sin(ax) + cos(bx) + tan(cx) $$

Q10.02 Create the symbolic math variables $a$, $b$, $c$ and $x$. Use these variables to define the symbolic math equations:

$$ ax^2 + bx = c $$

$$ \frac{sin(ax)}{cos(bx)} = tan(cx) $$

Q10.03 Create the symbolic math variables $a$, $b$, $c$, $x$, and $y$. Use these variables to define the symbolic math expression:

$$ ax^2 + bx + c $$

Substitute the variable $y$ in for the variable $c$.

Substitute the value ```5``` in for the variable $y$.

Q10.04 Create the symbolic math variables $E$, $A$, $d$, $P$, $L$, and $F$. Use these variables to define the symbolic math equation:

$$ d = \frac{PL}{AE} $$

Substitute the value $29 \times 10^6$ for $E$

Substitute $F/2$ for the variable $P$

Q10.05 Create the symbolic math variables $t$, $T$, $c$, and $J$. Use these variables to define the symbolic math equation:

$$ t = \frac{Tc}{J} $$

Substitute the $J = \frac{\pi}{2}c^4$ into the equation

Substitute $T=9.0$ and $c=4.5$. Print out the resulting value of $t$.

Q10.06 Mohr's circle is used in mechanical engineering to calculate the shear and normal stress. Given the height of Mohr's circle $\tau_{max}$ is equal to the expression below: 

$$ \tau_{max} = \sqrt{(\sigma_x - \sigma_y)/2)^2 + \tau_{xy}} $$ 

Use SymPy expressions or equations to calculate $\tau$ if $\sigma_x = 90$, $\sigma_y = 60$ and $\tau_{xy} = 20$

+++

#### Solving Equations

+++ {"latex": {"environment": "problems"}}

Q10.20 Use SymPy to solve for $x$ if $x - 4 = 2$

Q10.21 Use SymPy to solve for the roots of the quadratic equation $2x^2 - 4x + 1.5 = 0$

Q10.22 Create the symbolic math variable $b$ and define the equation below:

$$ \frac{1}{\sqrt{2}}(b - 6) = -1 $$

Find the numeric value of $b$ to three decimal places

Q10.30 Use SymPy to solve the system of linear equations below for the variables $x$ and $y$:

$$ -3x - 2y + 7  = 0 $$

$$ 5x - 3y - 6 = 0 $$

Q10.31 Use SymPy to solve the system of linear equations below for the variables $x$, $y$, and $z$:

$$ 2x + 4y - z = -0.6 $$

$$ -x - 3y + 2z = 2.2 $$

$$ \frac{1}{2}x + 6y - 3z = -6.8 $$

Q10.32 A set of five equations is below:

$$ -5x_1 - 4x_2 - 2x_3 + 2x_4 + 3x_5 = 10 $$

$$ 9x_1 + 3x_2 + 4x_3 + 10x_4 + 5x_5 = -5 $$

$$ 2x_1 + 4x_2 + 3x_3 + 2x_4 + x_5 = 12 $$

$$ 5x_1 - 4x_2 + 3x_3 - 2x_4 + 2x_5 = 32 $$

$$ x_1 - x_2 + 2x_3 + 4x_4 + 3x_5 = 42 $$

Use symbolic math variables and equations to solve for $x_1$, $x_2$, $x_3$, $x_4$ and $x_5$.

Q10.33 An equation in terms of the variables $L$ and $x$ is defined below.

$$ \frac{1}{6}L^3x^2 - \frac{1}{6}Lx^3 + \frac{1}{24}x^4 - \frac{1}{45}L^4 = 0 $$

Solve the equation for $x$ in terms of the variable $L$. Note their will be more than one solution.

Q10.50 Use SymPy to solve the system of non-linear equations below for the variables $x$ and $y$:

$$ 3x^2 + 2y^3 = -\frac{17}{4} $$

$$ \frac{-x^3}{2} - 8y^2 + \frac{127}{2} = 0 $$

```{code-cell} ipython3

```
