# python-api-challenge
Module 6

Final code for module 6 challenge is in WeatherPy_final.ipynb and VacationPy_final.ipynb.

The following resources were referenced to complete this challenge:

1. Add today's date - https://stackoverflow.com/questions/32490629/getting-todays-date-in-yyyy-mm-dd-in-python
2. Adjust plot title position - https://www.statology.org/matplotlib-title-position/
3. Add text inside plot and format text - https://www.geeksforgeeks.org/add-text-inside-the-plot-in-matplotlib/
4. Calculate linear regression - Instructor Eli Rosenberg covered this during class.
5. Add additional details to hover bubble - Instructor Eli Rosenberg covered this during class.
6. Drop empty rows in specific columns - https://www.w3resource.com/pandas/dataframe/dataframe-dropna.php
7. Geoapify hotel category - https://apidocs.geoapify.com/docs/places/#categories
8. Matplotlib edge color - https://stackoverflow.com/questions/45247486/how-to-do-a-scatter-plot-with-different-edgecolor-in-matplotlib
9. Matplotlib add grid - https://www.w3schools.com/python/matplotlib_grid.asp
10. Create python function - https://www.programiz.com/python-programming/function
11. API request loop - Starter code
12. Suppress .pyc files and _pycache_ folder - https://stackoverflow.com/questions/154443/how-to-avoid-pyc-files

## Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

### Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image

![image](https://github.com/patrickm96/python-api-challenge/assets/135382512/45e4b31d-fddb-4523-a976-9e2ea1d682ec)

You should create the following plots:

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

### Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

![image](https://github.com/patrickm96/python-api-challenge/assets/135382512/041b90f7-6a39-4a3e-8ec3-93831122e3f4)

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

![image](https://github.com/patrickm96/python-api-challenge/assets/135382512/6e904c8c-e1fe-4d75-b5c3-321f85b68963)

