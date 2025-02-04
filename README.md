# Geographic-environment-clustering-SQL
Grids on a map are clustered according to their road, building, population and sensor data characteristics

## Overview
Map grid (hexbins in this example) classification is required because radio performance is affected by environmental clutter. 
The presence of buildings (here used a single element of all possible street clutter), and movement and density of network users contribute to mobile network interference. 
When planning a radio network, the environment is therefore an important factor in the number of cells required to serve and area.

To assist with determing the required cell number, classify grid cells across the UK into categories Rural, Urban or Suburban. 
A K-means classification flags hexbins as Rural/Urban/Suburban.

<img width="869" alt="image" src="https://github.com/user-attachments/assets/ce88ddf2-4d1f-40f9-aac7-392e1c249413" />

Example of output across a Greater London area:

<img width="511" alt="image" src="https://github.com/user-attachments/assets/8b285e30-07a5-444a-b362-19378a51066d" />

## Requirements
Create the segments per the example requires the following data sources:
- mobile sensor data points (commercially available)
- buildings data (open source, e.g., OpenStreetMap)
- roads data (open source, e.g., Ordnance Survey)
- population data (open source, e.g., WorldPop)

## Code
The code provided is refernce material rather than ready to use, and illustrates the steps taken to achieve the sample output picture of Greater London, above
