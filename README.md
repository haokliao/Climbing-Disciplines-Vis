# Climbing-Disciplines - Data Vis Project
![](images/bouldering_img_1.png)

## Table of Contents 
* [General Info](#general-info)
* [Set Up](#set-up)
* [Technologies](#technologies)
* [To-do](#to-do)
* [Credits](#credits)


## General Info
This notebook file contains the code for my first project, an interactive data visualization heatmap in Seaborn done through Jupyter Notebooks with ipywidgets.

The goal of the project was to get a hands on experience with data vis in python, and I ended up choosing the Seaborn library to visualize my data as I wanted to take a learn as you go approach with it. 

The data I was working with was obtained through crowd sourcing my data, primarily from close friends and friends of friends through a social media survey, which ended up getting  a lot more than I was expecting! After retrieving the data, I had to "clean"/ try to quantify it better to make it more visually appealing for such a smaller sample size. 

Rock climbing is a sport that contains three different disciplines, with bouldering grades being measured from (v1 to v10+) and top rope and lead climbing measured using a (5') value. (To break it down simply, the higher the more difficult)
This chart showcases a very brief relationship between years climbing and grades in three different climbing disciplines (bouldering,top rope, and lead climbing) from a n=25, of climbers. 

Although it is a little overkill for this scale of a project, I managed to work with poetry to create a virtual environment so that you'd be able to have all your dependencies and package management done through a couple simple steps instead of going through the headache of trying to get proper versions. 

## Set Up

There are two different ways to set this up: 

1. You can run it locally through your own Jupyter Notebook, with the three CSV files and Seaborn installed.


2. To simplify the local installation, download [`poetry`](https://python-poetry.org/docs/#installation) and run in this folder.
```sh
poetry install
```
 The command above will setup a virtual environment with all the python dependencies you need to run the notebook (for this to work you need `python` v3.8 or higher in your system).

To create a new `requirements.txt` file, you can simply run
```sh
poetry export -f requirements.txt --output requirements.txt --without-hashes
```

Running the `CLIMBING.ipynb` notebook is then just as easy as   
```sh
poetry run jupyter lab CLIMBING.ipynb
```


## Technologies

Poetry - Python dependency management/package handling tool. Allows package dependencies to be installed in the right versions that we're using for this project and create a virtual environment.

Jupyter Notebook - Used to display and run the heatmaps

Ipywidgets - Interactive display, containing the different heatmaps for bouldering, toprope and lead through an accordian style widget.

Seaborn is a **required library to be able to run this project**, as it was the main library used and responsible for the heatmaps.

## To-do
- [x] Consolidate the seperate functions (bouldering, toprope, leadclimb)
- [x] Create poetry project for simpler installation
- [ ] Consolidate CSV files to a singular (dataframe?dictionary?)

## Credits 
Wanted to give a big thanks to @erinaldi for helping me with setting up and introducing me to Poetry, (as I was just going to force everyone to install seaborn on their own :))


Big big shoutout to @bhernandev for helping me with working through the ipywidgets documentation, and for [Schubert's](https://www.kaggle.com/spitfire2nd/enthusiast-to-data-professional-what-changes) kaggle notebook, which really inspired me to get my hands dirty with some data visualization and try my hand at an interactive heatmap. 
