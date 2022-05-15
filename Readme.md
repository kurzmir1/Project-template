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
According to literature wild boar sleep for around 12 hours in the forest during the day. The aim of this project is to find out whether this behavioural pattern can be detected in the movement data of wild boar. If the data shows that the wild boar stay in one place in the forest for about  12 hours, we would conclude that they are sleeping there during this time. 

## Research Questions
1. For how long do the tracked wild boar sleep on average?
2. Where do the wild boar sleep (forest or agricultural land)?

## Results / products
We expect that the data shows, that the tracked wild boar stay in one place in the forest for around 12 hours. We would then conclude that the wild boars are sleeping for approximately 12 hours on average.

## Data
We will use the wild boar data provided. Additionally, we need data about the habitats in the area. 

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
    
Procedure:
How long do the wild boar sleep?
- calculate distance between consecutive points of each individual
- filter for small values in distance between two consecutive points
- calculate the whole time span of one section with small values in distance
Where do the wild boar sleep?
- assign habitat to coordinates
- group "resting" trajectory parts by habitat
- put the selected sections of "resting" trajectories on a map with habitats in the background
- 
## Risk analysis
It might be difficult to distinguish between animals moving very slow and staying in one place? We would need to set a threshold.


## Questions? 
Threshhold for "small values in distance"?
Where can we get habitat data?

