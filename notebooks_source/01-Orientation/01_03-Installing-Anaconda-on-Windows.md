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

## Installing Anaconda on Windows

+++

For problem solvers, I recommend installing and using the Anaconda distribution of Python.

+++

This section details the installation of the Anaconda distribution of Python on Windows 10. I think the Anaconda distribution of Python is the best option for problem solvers who want to use Python. Anaconda is free (although the download is large which can take time) and can be installed on school or work computers where you don't have administrator access or the ability to install new programs. Anaconda comes bundled with about 600 packages pre-installed including **NumPy**, **Matplotlib** and **SymPy**. These three packages are very useful for problem solvers and will be discussed in subsequent chapters.

Follow the steps below to install the Anaconda distribution of Python on Windows.

#### Steps:

1. Visit [Anaconda.com/downloads](https://www.anaconda.com/download/)

2. Select Windows

3. Download the **_.exe_** installer

4. Open and run the **_.exe_** installer

5. Open the **Anaconda Prompt** and run some Python code

+++

#### 1. Visit the Anaconda downloads page

Go to the following link: [Anaconda.com/downloads](https://www.anaconda.com/download/)

The Anaconda Downloads Page will look something like this:

![The Anaconda distribution of Python download page](images/anaconda_download_page.png)

+++

#### 2. Select Windows

Select Windows where the three operating systems are listed.

![Anaconda downloads page. Windows download option is selected](images/anaconda_select_windows.png)

+++

#### 3. Download

Download the most recent Python 3 release. At the time of writing, the most recent release was the Python 3.6 Version. Python 2.7 is legacy Python. For problem solvers, select the Python 3.6 version. If you are unsure if your computer is running a 64-bit or 32-bit version of Windows, select 64-bit as 64-bit Windows is most common.

![Anaconda downloads page. Select Python 3.6 version or higher. Python 2 is legacy Python.](images/anaconda_python3_or_python2.png)

You may be prompted to enter your email. You can still download Anaconda if you click ```[No Thanks]``` and don't enter your Work Email address.

![Part of Anaconda installation. You don't have to enter your work email to proceed.](images/anaconda_enter_email.png)

The download is quite large (over 500 MB) so it may take a while to for Anaconda to download.

![Anaconda downloading.Note the file size and amount of time remaining](images/anaconda_downloading.png)

+++

#### 4. Open and run the installer

Once the download completes, open and run the **_.exe_** installer

![Once the download is complete, open the .exe file](images/anaconda_run_installer.png)

At the beginning of the install, you need to click **Next** to confirm the installation.

![Welcome to Anaconda3 installation screen. Click next to proceed with the installation.](images/anaconda_installer_click_next.png)

Then agree to the license.

![Anaconda End User License Agreement. Click I Agree to proceed](images/anaconda_agree_to_license.png)

At the Advanced Installation Options screen, I recommend that you **do not check** "Add Anaconda to my PATH environment variable"

![Anaconda installation options. When installing Anaconda on Windows, do not check Add Anaconda to my PATH environment variable](images/anaconda_path2.png)

+++

#### 5. Open the Anaconda Prompt from the Windows start menu

After the installation of Anaconda is complete, you can go to the Windows start menu and select the Anaconda Prompt.

![The Anaconda Prompt in the Windows Start Menu](images/anaconda_from_start_menu.png)

This opens the **Anaconda Prompt**. **Anaconda** is the Python distribution and the **Anaconda Prompt** is a command line shell (a program where you type in commands instead of using a mouse). The black screen and text that makes up the **Anaconda Prompt** doesn't look like much, but it is really helpful for problem solvers using Python.

At the Anaconda prompt, type ```python``` and hit ```[Enter]```. The ```python``` command starts the Python interpreter, also called the Python REPL (for Read Evaluate Print Loop).

```text
> python
```

![The Anaconda Prompt: What you see when you open the Anaconda Prompt. Note the word "python" was typed at the > prompt](images/conda_prompt_type_python.png)

Note the Python version. You should see something like ```Python 3.6.1```.  With the interpreter running, you will see a set of greater-than symbols ```>>>``` before the cursor. 

![The Anaconda Prompt: The result of typing python is the Python REPL opens. Note the >>> prompt which denotes the Python interpreter is running](images/conda_type_python.png)

Now you can type Python commands. Try typing ```import this```. You should see the **_Zen of Python_** by Tim Peters

![Anaconda Prompt: Results of entering import this is The Zen of Python, by Tim Peters](images/conda_import_this_output.png)

To close the Python interpreter, type ```exit()``` at the prompt ```>>>```.  Note the double parenthesis at the end of the ```exit()``` command. The ```()``` is needed to stop the Python interpreter and get back out to the **Anaconda Prompt**.

To close the **Anaconda Prompt**, you can either close the window with the mouse, or type ```exit```, no parenthesis necessary.

When you want to use the Python interpreter again, just click the Windows Start button and select the **Anaconda Prompt** and type ```python```.

```{code-cell} ipython3

```
