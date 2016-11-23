# R spatial workflow roadmap
Tim Appelhans, ...  
November 23, 2016  



## Introduction
Without too much babbling, this document is meant as a brainstorming place for collecting ideas and requirements for advancing spatial analysis workflow in R. The ultimate aim is, in my opinion, to enable a complete workflow for the day-to-day stuff from disk storage (I/O) to interactive data manipulation without the need to open external software. Hopefully there will be a pathway emerging from this collection and we can advance R's capabilities for spatial data analysis.

The document is organised accroding to the minimum main steps involved in spatial workflow. Please contribute by expanding this document in any way you see fit but try to be as concise and clear as possible. **If you have extended input to any of the major points, please provide a stand-alone document (rmd & html) and include a link to it in the main document at the relevant position.** Questions regrding unclear points should probably be made as an iussue referencing the main document.

To visualise the general idea of spatial workflow I have simplified the 'tidyverse' workflow model and added main packages involved in the individual steps.

![](minimum_workflow.svg)

Please note that this is far from complete so feel free to manipulate and adjust this svg file as you see fit...

## Import


## Manipulate


## Visualise
In this context visualise refers to quick visual inspection of data during workflow. For final presentation grade visualisations refer to section *Communicate*

This is what e.g. packages **mapview** and **qmapr** are written for (the latter can now be used within mapview by setting `mapviewOptions(platform = "qmapr")`. Package **tmap** has function `qtm()` for quick plotting/viewing.

### mapview
**mapview** currently does two things, it

1. visualises the data using leaflet and stores the leaflet map in slot `@map` and 
2. sotres the modifed object(s) that are visualied in a list in slot `@object` - 
the intention of this is to enable the user to track manipulations that have necessarily been carried out on the object(s) to correctly visualise it (e.g. re-projection).

A comprehensive overview of mapview functionality can be found [here](http://environmentalinformatics-marburg.github.io/mapview/introduction.html)



## Edit

## Communicate

