# Module 6 Challenge

In this modules challenge, First we have to create a repository named, python-api-challenge. This folder contains the jupyter notebook for weather data as well as vacation data. Api keys used in this challenge is hidden in the api_keys.py file. To make it hidden from others, we add the api_keys.py file to .gitignore. This way we can protect our api keys while still sharing our codes with others.


<img width="518" alt="Screenshot 2025-02-07 at 10 25 15 AM" src="https://github.com/user-attachments/assets/e2ed5420-44c5-465c-b942-27ff9750a5c5" />



 This challenge is broken down into two deliverables, WeatherPy and VacationPy.

 ## WeatherPy

 In this deliverable, we'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. We are using the OpenWeatherMap API to complete this challenge. Starter code, WeatherPy.ipynb is used to complete this task.

 weather_api_key is obtained from the OpenWeatherMap API. Use this key to retrieve weather data from the cities list generated in the starter code. 

 ### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

create a base_url using the api key and by passing required parameters. Save the cities generated as a CSV file to an output_data folder.
Read this csv file to do further comparisons. 

### Create the Scatter Plots Requested

Various scatter plots are generated using this data.

Latitude Vs. Temperature
Latitude Vs. Humidity
Latitude Vs. Cloudiness
Latitude vs. Wind Speed Plot

all the output images are saved inside the output_data folder.

We also calculated linear regression for each of these relationship.

### Requirement 2: Compute Linear Regression for Each Relationship

> Temperature vs. Latitude Linear Regression Plot

There is a negative correlation between latitude and temperature in northern hemisphere.
There is a slighter positive coorelation between latitude and temperature in southern hemisphere.

> Humidity vs. Latitude Linear Regression Plot

There is a slighter positive correlation between latitude and humidity in both northern and southern hemisphere.

> Cloudiness vs. Latitude Linear Regression Plot

There is a weak positive correlation between latitude and cloudiness in northern hemisphere.
There is a strong positive correlation between latitude and cloudiness in southern hemisphere.

> Wind Speed vs. Latitude Linear Regression Plot

There is a neglagible relation between latitude and wind speed in northern hemisphere.
There is a negative correlation between latitude and wind speed in southern hemisphere.


## VacationPy

In this deliverable, we'll use our weather data skills to plan future vacations. Also, we'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API key.

geoapify_key is used to store my geoapify key values. Read the cities.csv file from the output_data folder.

### Step 1: Create a map that displays a point for every city in the city_data_df DataFrame. The size of the point should be the humidity in each city.

using a hvplot.points, ew were able to pin point each and every coordinates. We can also pass other parameters like size, color, xlabel, ylabel etc to make the map looks more interesting.


![Screenshot 2025-02-05 at 11 13 01 PM](https://github.com/user-attachments/assets/57c580c0-3b3b-41e9-b997-e119483a60af)


### Step 2: Narrow down the city_data_df DataFrame to find your ideal weather condition

We are narrowing down the cities according to our personal preferences. 

### Step 3: Create a new DataFrame called hotel_df.

creating a new dataframe called hotel_df to store the city, country, coordinates and humidity details from cities.

### Step 4: For each city, use the Geoapify API to find the first hotel located within 10,000 metres of your coordinates.

geoapify_key is obtained from Geoapify.com. We can see the various parameters used to create our base URL.

<img width="651" alt="Screenshot 2025-02-05 at 11 20 17 PM" src="https://github.com/user-attachments/assets/c610764c-6d9c-4b9d-ae7c-ad0125101436" /> 

from the documentaion provided in the website we can choose various key combinations. Since we are looking for hotels, we choose accommodation.hotel as categories.

### Step 5: Add the hotel name and the country as additional information in the hover message for each city in the map.

last step is to show a map plot with hover values including the hotel name and country.


![Screenshot 2025-02-05 at 11 25 00 PM](https://github.com/user-attachments/assets/6414f801-6625-4614-9e5b-3889e221140e)


# Acknowledgment 

I have completed the challenge with the help of my Instructor and some internet searches.





