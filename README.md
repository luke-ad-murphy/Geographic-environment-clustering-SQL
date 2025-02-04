# Geographic Environment Clustering (SQL)

Grids on a map are clustered based on road, building, population, and sensor data characteristics.

## Overview

Classification of map grids (hexbins in this example) is important for understanding radio performance, as environmental clutter significantly impacts signal propagation. The presence of buildings, street clutter, and the movement and density of network users all contribute to mobile network interference.

When planning a radio network, environmental factors play a critical role in determining the number of cells required to serve a given area effectively.

## Objective

To optimize network planning, this project classifies grid cells across the UK into three categories: Rural, Urban, and Suburban. Using a K-means clustering algorithm, hexbins are categorized based on their environmental characteristics to aid in estimating the required number of radio cells for optimal coverage and performance.

## Features

-- Environmental Clustering: Uses road, building, population, and sensor data to categorize regions.
-- Hexbin-Based Classification: Employs hexagonal binning for spatial analysis.
-- K-Means Algorithm: Performs unsupervised clustering to classify regions into Rural, Urban, and Suburban.

## Use Cases
- Mobile Network Planning: Estimating the number of cells needed for optimal coverage.
- Urban Development Analysis: Understanding population density and infrastructure impact.
- Geospatial Research: Studying environmental clustering and its effects on connectivity.

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
