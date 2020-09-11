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

## What is a Jupyter Notebook?

+++

A _Jupyter notebook_ is an electronic file that contains both programming code and text descriptions. Jupyter notebooks can also contain embedded charts, plots, images, videos, and links. Jupyter notebooks run in a web browser like Firefox or Google Chrome.

+++

Although Jupyter notebooks can contain the code of many different programming languages, many Jupyter notebooks contain Python code. The Python code in a Jupyter notebook is the same type of Python code found in a **_.py_** file.

The text description sections of Jupyter notebooks contain explanations and clarifications of the programming code in the _markdown_ format. _Markdown_ files have the extension **_.md_**. Markdown sections of a Jupyter notebook can include formatting to make text bold, italic, form tables and lists, show code listings and render images.

+++

One way to think of a Jupyter notebook is as a combination of the Python REPL and a Python module **_.py_** file with a markdown **_.md_** file thrown in between code sections. 

In the Python REPL, only one command can be typed at a time, and only one line of output is shown at a time. In a **_.py_** file, the entire file is run at one time, line by line. The output of the entire file is produced all at once. Markdown **_.md_** files contain text in markdown format, but that text is not rendered. In a Jupyter notebook, chunks of code one line or many lines long can be run individually and in any order without running all of the code in the Jupyter notebook. Jupyter notebooks render the markdown sections and display rich text with headings, formatting, and images.

+++

Jupyter notebooks contain three types of cells: _code cells_, _output cells_, and _markdown cells_. 

 * Code cells: Lines of Python code are run in code cells.
 
 * Output cells: The output from running the code cells is also shown in output cells. Charts, plots, command line output, and images can all be shown in Jupyter notebooks as well.
 
 * Markdown cells: Contain text-like descriptions of what will happens in subsequent code cells. Markdown cells can also contain images and links.
 

```{code-cell} ipython3

```
