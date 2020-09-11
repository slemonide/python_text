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

## Installing Juypter

+++

The simplest way to install **Jupyter notebooks** is to download and install the Anaconda distribution of Python. The Anaconda distribution of Python comes with Jupyter notebook included and no further installation steps are necessary.

Below are additional methods to install Jupyter notebooks if you are not using the Anaconda distribution of Python.

+++

### Installing Jupyter on Windows using the Anaconda Prompt

To install Jupyter on Windows, open the **Anaconda Prompt** and type:

```text
> conda install jupyter
```

Type ```y``` for yes when prompted. Once Jupyter is installed, type the command below into the **Anaconda Prompt** to open the Jupyter notebook file browser and start using Jupyter notebooks.

```text
> jupyter notebook
```

+++

### Installing Jupyter on MacOS

To install Jupyter on MacOS, open the MacOS terminal and type:

```text
$ conda install jupyter
```

Type ```y``` for yes when prompted.

If **conda** is not installed, the Anaconda distribution of Python can be installed, which will install **conda** for use in the MacOS terminal.

Problems can crop up on MacOS when using the MacOS provided system version of Python. Python packages may not install on the system version of Python properly. Moreover, packages which do install on the system version of Python may not run correctly. It is therefore recommended that MacOS users install the **Anaconda** distribution of Python or use **homebrew** to install a separate non-system version of Python. 

To install a non-system version of Python with **homebrew**, key the following into the MacOS terminal. See the **homebrew** documentation at [https://brew.sh](https://brew.sh/).

```text
$ brew install Python
```

After **homebrew** installs a non-system version of Python, **pip** can be used to install Jupyter.

```text
$ pip install jupyter
```

+++

### Installing Jupyter on Linux

To install Jupyter on Linux, open a terminal and type:

```text
$ conda install jupyter
```

Type ```y``` for yes when prompted.

Alternatively, if the Anaconda distribution of Python is not installed, one can use **pip**.

```text
$ pip3 install jupyter
```

```{code-cell} ipython3

```
