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

# Virtual Environments

+++

Using _virtual environments_ is standard practice in Python. A virtual environment is an isolated installation of Python with associated packages. When you use virtual environments, one project can have a separate version of Python and packages. Another project can use a different virtual environment and therefore have a different version of Python and a different set of packages. 

Two projects on the same computer can use different versions of Python and different versions of packages if virtual environments are used.

+++

## Create a virtual environment with the Anaconda Prompt

To create the new virtual environment, open the **Anaconda Prompt** and issue the command:

```text
> conda create --name env_name python=3.7
```

The ```conda create``` command builds the new virtual environment. The ```--name env_name``` flag gives the new virtual environment the name ```env_name```.  Including ```python=3.7``` ensures the virtual environment has a current version of Python. 

The following output or something similar results:

```text
The following NEW packages will be INSTALLED:

  ca-certificates    ca-certificates-2019.5.15-0
  certifi            certifi-2019.6.16-py37_0
  openssl            openssl-1.1.1c-he774522_1
  pip                pip-19.1.1-py37_0
  python             python-3.7.3-h8c8aaf0_1
  setuptools         setuptools-41.0.1-py37_0
  sqlite             sqlite-3.28.0-he774522_0
  vc                 vc-14.1-h0510ff6_4
  vs2015_runtime     vs2015_runtime-14.15.26706-h3a45250_4
  wheel              wheel-0.33.4-py37_0
  wincertstore       wincertstore-0.2-py37_0
```

Type ```y``` to confirm and create the new virtual environment. 

+++

## Activate a virtual environment

To use the new virtual environment ```env_name```, the virtual environment needs to be _activated_. To activate the environment ```env_name```, issue the command:

```text
> conda activate env_name
```

The virtual environment is active when you see ```(env_name) >``` in parenthesis at the start of the prompt.

```text
(env_name) > 
```

+++

## Install packages in a virtual environment

When a new virtual environment is created, no packages are installed by default. If you use the Anaconda distribution of Python, the ```base``` environment contains about 600 packages that come with Anaconda. But a fresh new virtual environment will just have Python installed, no other packages.

To install a package into the virtual environment ```env_name```, first make sure the environment is active (```(env_name)``` before the prompt). Then package installation is accomplished with the ```conda install``` command followed by the package name. To install Matplotlib into a virtual environment type:

```text
(env_name) > conda install matplotlib
```

Multiple packages can be installed with the same command. To install both NumPy and Jupyter at the same time use:

```text
(env_name) > conda install numpy jupyter
```

+++

## Deactivate a virtual environment

To deactivate an active environment, run the command:

```text
(env_name) > conda deactivate
>
```

When the virtual environment is deactivated, the prompt looks normal (just ```>```), with no environment name in parenthesis before it.

+++

## List your virtual environments

View a list of your virtual environments using the command ```conda info --envs``` or ```conda env list```.

```text
> conda activate env_name
(env_name) > conda info --envs

# conda environments:
#
base                     /home/tribilium/anaconda3
env_name               * /home/tribilium/anaconda3/envs/env_name
matplotlib               /home/tribilium/anaconda3/envs/matplotlib
```

Notice the ``` * ``` asterisk on the line with ```env_name```. The virtual environment with the ``` * ``` is currently active. 

To exit the virtual environment, use the command ``` conda deactivate```. 

```text
(env_name) > conda deactive
```

If you run ```conda info --envs``` again, there is no ```*``` in front of ```env_name```. That's because the ```env_name``` virtual environment is no longer active.

```text
> conda info --envs

# conda environments:
#
base                  *  /home/tribilium/anaconda3
env_name                 /home/tribilium/anaconda3/envs/env_name
matplotlib               /home/tribilium/anaconda3/envs/matplotlib

```

+++

## Remove a virtual environment

Remove a virtual environment with the command ```conda remove --name env_name --all```. You need to exit out of the environment before you remove it.

Check to see if the virtual environment you want to remove is present:

```text
> conda info --envs

# conda environments:
#
base                  *  /home/tribilium/anaconda3
env_name                 /home/tribilium/anaconda3/envs/env_name
matplotlib               /home/tribilium/anaconda3/envs/matplotlib

```

Remove the virtual environment called ```env_name``` using the command.

```text
> conda remove --name env_name --all

Proceed ([y]/n)?
```

Type [y] to remove the environment. Now view a list of your virtual environments again. Note that ```env_name``` is no longer in the list.

```text
> conda info --envs

# conda environments:
#
base                  *  /home/tribilium/anaconda3
matplotlib               /home/tribilium/anaconda3/envs/matplotlib

```

```{code-cell} ipython3

```
