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

# Installing Matplotlib

+++

Before Matplotlib's plotting functions can be used, Matplotlib needs to be installed. Depending on which distribution of Python is installed on your computer, the installation methods are slightly different.

+++

## Use the Anaconda distribution of Python

The simplest way to install Matplotlib is to download and install the Anaconda distribution of Python. The Anaconda distribution of Python comes with Matplotlib pre-installed and no further installation steps are necessary.

Below are additional methods to install Matplotlib if you are not using the Anaconda distribution of Python.

+++

## Install Matplotlib with the Anaconda Prompt

Matplotlib can be installed using with the **Anaconda Prompt**. If the **Anaconda Prompt** is available on your machine, it can usually be seen in the Windows Start Menu. To install Matplotlib, open the **Anaconda Prompt** and type:

```text
> conda install matplotlib
```

Type ```y``` for yes when prompted.

+++

## Install Matplotlib with **pip**

Matplotlib can also be installed using the Python package manager, **pip**. To install Matplotlib with **pip**, open a terminal window and type:

```text
$ pip install matplotlib
```

This command installs Matplotlib in the current working Python environment.

+++

## Verify the installation

+++

To verify that Matplotlib is installed, try to invoke Matplotlib's version at the Python REPL. Use the commands below that include calling the ```.__version__``` an attribute common to most Python packages.

+++

```python
>>> import matplotlib
>>> matplotlib.__version__
'3.1.1'
```

```{code-cell} ipython3

```
