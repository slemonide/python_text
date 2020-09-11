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

## The Anaconda Distribution of Python

+++

I recommend problem solvers install the _Anaconda distribution of Python_. The following section details the differences between the Anaconda distribution of Python and the version of Python you can download from [Python.org](https://python.org)

+++

### How is Anaconda different from Python?

When you download Python from Python.org, you get the _Python Interpreter_, a little text editing program called **IDLE** and all of the Python Standard Library modules. 

The Python Interpreter is an application or program that runs your Python code. A program written in the Python programming language is run with the Python Interpreter. So Python corresponds to both the language that a program is written in as well as the application that runs the program.

When you download the Anaconda distribution of Python from Anaconda.com, you get a Python Interpreter, the **Anaconda Prompt** (a command line program), **Spyder** (a code editor) and about 600 extra Python modules that aren't included in the Python Standard Library. The Anaconda distribution of Python also includes a program called Anaconda Navigator that allows you to launch Jupyter notebooks quickly.

+++

### Why download Anaconda, if I want to use is Python?

Regardless if you download Python from Python.org or if you download Anaconda (with all the extra stuff it comes with) from Anaconda.com, you will be able to write and execute Python code. However, there are a couple of advantages to using the Anaconda distribution of Python.

#### Anaconda includes Python plus about 600 additional Python packages

The Anaconda distribution of Python is advantageous because it includes Python as well as about 600 additional Python packages. These additional packages are all free to install. The packages that come with Anaconda includes many of the most common Python packages use to solve problems. If you download Anaconda, you get Python including the Python Standard Library plus about 600 extra packages. If you download Python from Python.org, you just get Python and The Standard Library but no additional modules. You could install the extra modules that come with Anaconda (that don't come with plain old Python), but why not save a step (or about 600 steps) and just install Anaconda instead of installing about 600 different modules?

#### Anaconda installs without administrator privileges

Even if you don't have the ability to install programs on a computer, like a computer in a school computer lab, you can still download and use Anaconda. The Anaconda distribution of Python will also allow you to install additional modules from the Python package index ([PyPI.org](https://pypi.org/)) and conda-forge ([conda-forge.org](https://conda-forge.org/)), the conda package index.

#### Anaconda works on MacOS

If you use MacOS, you probably already have Python installed on your computer. Most MacOS installations come with Python included. The problem is that the version of Python that comes with MacOS is old (usually legacy Python, Python 2) and the version of Python that comes with MacOS is locked up behind a set of administrator privileges. Because the pre-installed version of Python included with MacOS can require administrator privileges, you can have trouble with installation and run-time problems. Some things will seem to work fine, and then other things won't run at all, or you will keep getting asked for an administrator password over and over. 

Downloading and installing Anaconda (separate from the version of Python that came with MacOS) prevents most of the problems on MacOS caused by using the pre-installed version of Python.

#### Anaconda makes package management and virtual environments easier

Another advantage of Anaconda is that package management and virtual environments are a lot easier when you have Anaconda. Virtual environments and package handling might not seem to make a huge difference right now. If you just downloaded Anaconda for the first time, you are probably not dealing with package management and virtual environments yet. (It's OK if you don't even know what those two things are yet). After you write a couple of Python programs and start downloading a couple of extra modules from PyPI or conda-forge, dealing with package management and virtual environments becomes more critical.

```{code-cell} ipython3

```
