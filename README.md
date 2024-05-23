# Python API Challenge: Weather Analysis and Vacation Planning

## Overview

This project leverages the power of data to answer the fundamental question: "What is the weather like as we approach the equator?" Using Python, APIs, and data visualization tools, we will analyze weather data from over 500 cities to understand weather patterns and plan ideal vacation spots based on specific weather criteria.

## Table of Contents
- [Background](#background)
- [Dataset](#dataset)
- [Project Tasks](#project-tasks)
  - [1. WeatherPy](#1-weatherpy)
    - [Requirement 1: Create Plots to Showcase Weather Variables](#requirement-1-create-plots-to-showcase-weather-variables)
    - [Requirement 2: Compute Linear Regression](#requirement-2-compute-linear-regression)
  - [2. VacationPy](#2-vacationpy)
    - [Requirement 1: Map Cities](#requirement-1-map-cities)
    - [Requirement 2: Find Ideal Vacation Spots](#requirement-2-find-ideal-vacation-spots)
- [Results Summary](#results-summary)
- [Conclusion](#conclusion)

## Background

Data's true power lies in its ability to answer questions definitively. This project involves analyzing weather data to explore the relationship between latitude and various weather conditions, ultimately aiding in planning ideal vacation spots.

## Dataset

The dataset comprises weather data retrieved from the OpenWeatherMap API for over 500 cities around the world. The data includes information on temperature, humidity, cloudiness, and wind speed.

## Project Tasks

### 1. WeatherPy

In this part of the project, we will visualize weather data for cities located at various distances from the equator.

#### Requirement 1: Create Plots to Showcase Weather Variables

**Objectives:**
- Retrieve weather data for a list of cities using the OpenWeatherMap API.
- Create scatter plots to showcase the relationships between latitude and the following weather variables:
  - Temperature
  - Humidity
  - Cloudiness
  - Wind Speed

**Steps:**
1. Use the `citipy` library to generate random geographic coordinates and find the nearest city for each coordinate.
2. Use the OpenWeatherMap API to retrieve weather data for each city.
3. Create scatter plots to visualize the relationship between latitude and each weather variable.

#### Requirement 2: Compute Linear Regression

**Objectives:**
- Compute linear regression for the relationships between latitude and each weather variable.
- Separate the data into Northern and Southern Hemispheres for analysis.

**Steps:**
1. Create functions to compute and plot linear regression for each relationship.
2. Generate scatter plots with regression lines for the following:
   - Northern Hemisphere: Temperature vs. Latitude
   - Southern Hemisphere: Temperature vs. Latitude
   - Northern Hemisphere: Humidity vs. Latitude
   - Southern Hemisphere: Humidity vs. Latitude
   - Northern Hemisphere: Cloudiness vs. Latitude
   - Southern Hemisphere: Cloudiness vs. Latitude
   - Northern Hemisphere: Wind Speed vs. Latitude
   - Southern Hemisphere: Wind Speed vs. Latitude
3. Interpret the results and describe any observed relationships.

### 2. VacationPy

In this part of the project, we will use weather data to plan ideal vacation spots based on specific weather criteria.

#### Requirement 1: Map Cities

**Objectives:**
- Create a map that displays a point for every city in the dataset, with the point size representing the humidity in each city.

**Steps:**
1. Load the weather data into a DataFrame.
2. Use the `geoViews` library to create a map visualization.

#### Requirement 2: Find Ideal Vacation Spots

**Objectives:**
- Identify cities with ideal weather conditions for a vacation.
- Find nearby hotels for each selected city using the Geoapify API.

**Steps:**
1. Define criteria for ideal vacation weather (e.g., temperature range, wind speed, cloudiness).
2. Filter the dataset to find cities that meet these criteria.
3. Create a new DataFrame to store the city, country, coordinates, and humidity.
4. Use the Geoapify API to find the first hotel within 10,000 meters of each city's coordinates.
5. Add the hotel name and country to the DataFrame.
6. Create a map visualization with hover information displaying the hotel name and country.

## Results Summary

**Key Findings:**
- Scatter plots and regression analysis reveal trends between latitude and weather variables such as temperature, humidity, cloudiness, and wind speed.
- Specific cities meeting the ideal weather criteria for vacations are identified and mapped, with nearby hotels highlighted.

**Visualizations:**
- Scatter plots for each weather variable vs. latitude.
- Linear regression plots for Northern and Southern Hemispheres.
- Maps showing humidity distribution and ideal vacation spots with hotel information.

## Conclusion

This project demonstrates the use of APIs and data visualization to analyze weather patterns and plan vacations based on specific criteria. The insights gained from this analysis can help travelers make informed decisions about their travel destinations.

---

This ReadMe case study outlines the methodology and findings of the weather analysis and vacation planning project, showcasing the application of Python, APIs, and data visualization techniques in real-world data analytics.
