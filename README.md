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
### macOS installation
SLiM can be installed on macOS using a prebuilt installer which can be downloaded [here](https://github.com/MesserLab/SLiM/releases/download/v4.3/SLiM_OSX_Installer.pkghttps://messerlab.org/slim/). Running the installer will install both, SLiMgui as well as EidosScribe. 
### Linux installation
Messerlabs provides a bash script 
