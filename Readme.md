# Proposal for Semester Project

**Patterns & Trends in Environmental Data / Computational Movement
Analysis Geo 880**

| Semester:      | FS22                              |
|----------------|---------------------------------- |
| **Data:**      | Wild Boar Movement Data           |
| **Title:**     | Wild boar sleeping behaviour         |
| **Student 1:** | Nina Poglic                |
| **Student 2:** | Mirjam Kurz                 |

## Abstract 
<!-- (50-60 words) -->

## Research Questions
1. For how long do the wild boar sleep?
2. Where do the wild boar sleep (forest or agricultural land)?

## Results / products
According to literature wild boar sleep for around 12 hours in the forest during the day. We expect to find this movement pattern in our data after the analysis.

## Data
We will use the wild boar data provided. Additionally, we need data about the habitats in the area. Can we get it from the geoportal of Bern?

## Analytical concepts
Conceptual movement space:
- Movement spaces: continuous movement spaces
- Properties of the movement: non-limited, active
- Perspective of observation: Lagrange (GPS)

Modelling approach of trajectories:
- sort trajectory parts into "moving" and "resting"
- calculate time spent "resting"

Spatial analysis method:
- in what space are the "resting" trajectory parts


## R concepts
packages:
- readr    
- dplyr 
- ggplot2
- sf
- terra
- lubridate
- tidyverse   
    
R concepts:
How long do the wild boar sleep?
- calculate distance between consecutive points
- filter for small values in distance between two consecutive points
- calculate the whole time span of one section with small values in distance
Where do the wild boar sleep?
- assign habitat to coordinates
- group "resting" trajectory parts by habitat
- put the selected sections of "resting" trajectories on a map with habitats in the background


<!-- Which R concepts, functions, packages will you mainly use. What additional spatial analysis methods will you be using? -->

## Risk analysis
It might be difficult to distinguish between animals moving very slow and staying in one place?
<!-- What could be the biggest challenges/problems you might face? What is your plan B? -->

## Questions? 
Threshhold for "small values in distance"?
Where can we get habitat data?
<!-- Which questions would you like to discuss at the coaching session? -->
