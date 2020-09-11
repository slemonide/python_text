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

+++ {"latex": {"before_cell": "newpage"}}

# Summary

+++

In this chapter, you learned how to create plots using Python and Matplotlib. You learned what Matplotlib is and why problem solvers should learn how to use Matplotlib. Matplotlib installation was shown at the start of the chapter. Then, you learned how to build line plots and save plots as image files. You learned how to customize plots by including axis label, titles, and legends on your plots. You also learned how to add annotations to plots.

The types of plots detailed in this chapter are shown in the table below.

| Chart Type | Matplotlib method |
| --- | --- |
| line plot | ```ax.plot(x,y)``` |
| multi-line plot | ```ax.plot(x,y) ax.plot(x,z)``` |
| bar graph | ```ax.bar(x_pos, heights)``` |
| pie chart | ```ax.pie(sizes, labels=[labels])``` |
| bar graphs with error bars | ```ax.bar(x_pos, heights, yerr=[error])``` |
| line plot with error bars | ```ax.errorbar(x, y, xerr= , yerr= )``` |
| histogram | ```ax.hist(data, n_bins)``` |
| box plot | ```ax.boxplot([data list])``` |
| violin plot | ```ax.violinplot([data list])``` |
| scatter plot | ```ax.scatter(x_points, y_points)``` |
| plot annotations | ```ax.annotate('text',xy=loc,xy_coords= )``` |
| subplots | ```fig, (ax1,ax2,ax3) = plt.subplots(1,3)``` |
| plot styles | ```plt.style.use('style')``` |
| 2D contour plot | ```ax.contour(X, Y, Z)``` |
| 2D filled contour plot | ```ax.contourf(X, Y, Z)``` |
| color bars | ```fig.colorbar(cf, ax=ax)``` |
| color maps | ```mycmap = plt.get_cmap('map')``` |
| quiver plot | ```ax.quiver(x_pos, y_pos, x_dir, y_dir)``` |
| stream plot | ```ax.streamplot(x,y,x_d,y_d, density= )``` |
| 3D surface plot | ```ax.plot_surface(X, Y, Z)``` |
| 3D wireframe plot | ```ax.plot_wireframe(X,Y,Z)``` |

+++

## Key Terms and Concepts

+++ {"latex": {"environment": "key_terms"}}

plot

dpi

invoke

library

parameters

RGBA

object

attribute

object-oriented programming

method

image resolution

error bars

box plot

violin plot

histogram

annotation

reference frame

contour plot

quiver plot

stream plot

gradient

field

wire frame plot

projection

+++

## Additional Resources

+++

Matplotlib official documentation: [https://matplotlib.org/contents.html](https://matplotlib.org/contents.html)

Matplotlib summary notebook on Kaggle: [https://www.kaggle.com/grroverpr/matplotlib-plotting-guide/notebook](https://www.kaggle.com/grroverpr/matplotlib-plotting-guide/notebook)

Python Plotting With Matplotlib (Guide) on Real Python: [https://realpython.com/python-matplotlib-guide/#why-can-matplotlib-be-confusing](https://realpython.com/python-matplotlib-guide/#why-can-matplotlib-be-confusing)

Python For Data Science: Matplotlib Cheat Sheet from DataCamp: [https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Matplotlib_Cheat_Sheet.pdf](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Matplotlib_Cheat_Sheet.pdf)

```{code-cell} ipython3

```
