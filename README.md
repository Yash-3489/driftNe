# Can the effects of genetic drift be large, even in a large population? 
Genetic drift is known to be inversely proportional to population size. Are there specific evolutionary conditions, however, under which this relationship stops holding true? Here we explore a few such factors, which contribute to a large effect of genetic drift, even in large populations.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Data analysis](#data_analysis)

## Introduction
Evolution is a genetic process, with the following as the four mechanisms of evolution: natural selection; genetic drift; mutation & migration. Out of these, drift particularly fascinates me, as it is always present in the background, irrespective of the other mechanisms at play. Also, very few sites in a genome actually code for proteins, and are directly under selection. However, _all_ sites undergo drift, making it all the more relevant. 
Drift is inversely proportional to population size. Here I'm interested at looking for such factors which can cause the effects of drift to be large, even in large popoulations. I'm using a forward genetic simulations based approach using the [SLiM software](https://messerlab.org/slim/) (Selection on Linked Mutation) to run the simulations. This software has specifically been designed to run population level genetic simulations. 

## Installation
### SLiM
The [SLiM Manual](https://github.com/MesserLab/SLiM/releases/download/v4.3/SLiM_Manual.pdf) provides a detailed installation guide for installations on all major platforms. 
SLiM version 4.3 has been used for all the code here. 

### R
R version 4.4.2 was used for this project, with RStudio as the IDE. 
- *Windows installation:* The latest version of R, as well as previous versions are available for download on windows [here](https://cran.r-project.org/bin/windows/base/)
- *Linux installations:* Various installations based on different distros can be found [here](https://cran.r-project.org/bin/)
- *macOS:* R installation files can be downloaded directly from [here](https://cran.r-project.org/bin/macosx/) for macOS and older versions of mac.

## Usage
### SLiM
SLiM is the software used for running the simulations and generating whole genome sequences. This software has its own language, Eidos, with many similarities and inbuilt functions like R, along with those specific to the simulation environment. The learning curve for a person unfamiliar with coding will be steep, as SLiM doesn't have intuitive syntax, and a lot of other functions which are specific to this framework. 
**Basic structure:**
- ```initialize()``` The very first code chunk, which defines all the conditions for the simulation. This includes, but is not limited to genome size, mutation rate, recombination rate, genome and mutation types.
- ```1 early()``` The first code chunk after the initialize chunk where all the starting conditions of the simulation are defined. This includes populations, population structures (migration rates), etc.
- ```late()``` Last chunk of the code, which marks the end of the simulation, and determines the number of generations the simulation runs for. Any outputs desired at the end of the simulation go in here.

Apart from this, a lot of other modifications can be made to the code, depending on the proficiency of the user. Log files (which I've used a lot) can be created to monitor population/individual parameters across generations. 
