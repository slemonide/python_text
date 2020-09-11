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

# Problem Solving with Python Book Construction

+++

## Jupyter Notebooks

+++

This book was constructed using Jupyter notebooks. The GitHub.com repo for the book can be found at:
    
 > [github.com/ProfessorKazarinoff/Problem-Solving-with-Python-37-Edition](https://github.com/ProfessorKazarinoff/Problem-Solving-with-Python-37-Edition)

+++

The directory structure of the GitHub repo contains all the Jupyter notebooks used the write the book. The repo also contains a set of custom conversion scripts and templates which convert the Jupyuter notebooks into **_.html_** and **_.tex_** files.

+++

```text
Problem-Solving-with-Python-37-Edition/
|-- conversion_tools/
|-- notebooks/
|-- LICENSE
|-- notebooks/
|-- pdf/
|-- README.md
|-- website/
```

+++

The ```notebooks``` directory contains a directory for each chapter of the book:

+++

```text
notebooks/
|-- 00-Preface/
|-- 01-Orientation/
|-- 02-Jupyter-Notebooks/
|-- 03-The-Python-REPL/
|-- 04-Data-Types-and-Variables/
|-- 05-Matrices-and-Arrays/
|-- 06-Plotting-with-Matplotlib/
|-- 07-Functions-and-Modules/
|-- 08-If-Else-Try-Except/
|-- 09-Loops/
|-- 10-Symbolic-Math/
|-- 11-Python-and-External-Hardware/
|-- 12-MicroPython/
|-- 99-Appendix/
`-- figures/
```

There is a Jupyter notebook for each section of the book within each chapter directory. Each chapter directory contains an ```images``` directory for any images used in the markdown cells of the notebooks.

```text
01-Orientation/
|-- 01.00-Welcome.ipynb
|-- 01.01-Why-Python.ipynb
|-- 01.02-The-Anaconda-Distribution-of-Python.ipynb
|-- 01.03-Installing-Anaconda-on-Windows.ipynb
|-- 01.04-Installing-Anaconda-on-MacOS.ipynb
|-- 01.05-Installing-Anaconda-on-Linux.ipynb
|-- 01.06-Installing-Python-from-Python-dot-org.ipynb
|-- 01.07-Summary.ipynb
|-- 01.08-Review-Questions.ipynb
`-- images/
```

+++

## Website

+++

The website for this book was constructed using **Mkdocs** (https://www.mkdocs.org) and the **Material for MkDocs** (https://squidfunk.github.io/mkdocs-material/) theme. Jupyter noteboks were exported to **_.html_** files with markdown cells unformatted using a custom script and **nbconvert**.

+++

## Hardcopy

+++

The hard copy of the book was constructed using LaTeX, **nbconvert** and a set of custom scripts and templates. One conversion script combined all of the notebooks into one BIG notebook.  The BIG notebook was then converted into LaTeX using **nbconvert** and a custom template. Outside of the Python ecosystem, a separate installation of TeXworks compiled the LaTeX **_.tex_** file to a **_.pdf_** document.

```{code-cell} ipython3

```
