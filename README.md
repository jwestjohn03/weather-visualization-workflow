# Automated Weather Visualization Pipeline

## Overview
This project is an automated data workflow that uses the OpenWeather API to collect, process, and visualize historical weather data across U.S. states. It enables comparative analysis between two user-defined years and generates geospatial choropleth maps for key climate variables.

The system supports:
- Temperature (°F)
- Wind speed (mph)
- Humidity (%)
- Year-over-year difference analysis

## Features
- User-defined year selection (e.g., 2000 vs 2025)
- Automated API data collection across all U.S. states
- State-level aggregation of weather metrics
- Interactive choropleth maps using Plotly
- Difference maps showing climate change between years

## Workflow

1. **Data Collection**
   - Fetches daily weather data from OpenWeather API
   - Iterates over U.S. states and time range (Jan 1 – Dec 31)

2. **Data Processing**
   - Converts raw API output into structured dataset
   - Computes derived metrics (°F, mph)
   - Aggregates data by state and year

3. **Analysis**
   - Computes state-level averages
   - Separates datasets by user-selected years

4. **Visualization**
   - Generates choropleth maps for each variable
   - Produces difference maps (Year2 − Year1)
