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

## Installation and version info
### SLiM
The [SLiM Manual](https://github.com/MesserLab/SLiM/releases/download/v4.3/SLiM_Manual.pdf) provides a detailed installation guide for installations on all major platforms. 
SLiM version 4.3 has been used for all the code here. 

### R
R version 4.4.2 was used for this project, with RStudio as the IDE. 
- *Windows installation:* The latest version of R, as well as previous versions are available for download on windows [here](https://cran.r-project.org/bin/windows/base/)
- *Linux installations:* Various installations based on different distros can be found [here](https://cran.r-project.org/bin/)
- *macOS:* R installation files can be downloaded directly from [here](https://cran.r-project.org/bin/macosx/) for macOS and older versions of mac.

## Usage
