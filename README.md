# https://github.com/story645/pydata_nyc_2023/

In this tutorial we will explore the Palmer Penguins dataset, starting with exploratory charts, then creating a linked animation, and concluding with converting the animation into a simple interactive visualization. In doing so, this tutorial will unpack some of the fundamental concepts that underlie the architecture of Matplotlib, hopefully providing attendees with the foundation for creating effective visualizations using Matplotlib.

Matplotlib is a big library, and it can be difficult to know where to start. This tutorial is a guided tour through many of the essential features and concepts of Matplotlib so you can get started making publication-quality, animated, and interactive figures. We will be using the Penguins digit dataset as a case study.

### Get started

`git clone` this repo locally or open codespaces
  
If cloned locally, create the conda environment by going into the folder and typing:
```
path\to\pydata_nyc> conda env create -f environment.yml
```
then activate the environment
```
path\to\pydata_nyc> conda activate pynyc23
```
then install the jupyter interactive extensions:

```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install jupyter-matplotlib
```
then open jupyterlab inside this folder:

```
path\to\pydata_nyc>(pynyc) jupyter lab
```

Then go to [notebook 1: static visualizations]()

### Data acknowledgement 
The data is included here from ease of use, but it is a direct copy paste of penguins in https://github.com/mwaskom/seaborn-data

### Schedule
This schedule/dataset is subject to change, but the rough plan is:

start up: [10 minutes]
- verify install/open codespaces/get settled
- What most intrigues you at https://matplotlib.org/devdocs/gallery/index.html
 - add link to shared notes: https://hackmd.io/@story645/pynyc23 

Introduction [20 minutes]
- figure→axes→elements diagram
-Example: plot a heatmap/matshow of penguins
- Together: scatter plot of bill_length_mm vs bill_depth color by species and vary by size
Exercise: (I'll show the finished figure)
- subplot mosaic -> add an empty axes
- add a bar chart showing the mean of each variable
- add labels

Animation[25 minutes]
- example: highlight one penguin on heatmap, scatter, and bar chart
- example: movie highlighting each penguin on the heatmap
- add in highlighting on the scatter
- exercise: [10 minute]
linked movie highlighting each penguin on bar chart

Interactivity: [30 minutes]
- break scatter out by species and show out of the box linked zoom
- use jupyter widgets to slide the animation
- custom interactivity to select the penguin on the heatmap and update the bar chart
- exercise[15 minutes]
- select the penguin in the scatter plot and update the bar chart

Wrap up: [5 minutes]
- overview of resources for how to go further
