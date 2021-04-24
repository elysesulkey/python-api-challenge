# python-api-challenge
WeatherPy is a Python script that visualizes the weather of 500+ cities across the world of varying distance from the equator, utilizing the OpenWeatherMap API. 

The script first makes scatter plots to examine the following relationships:

    Temperature (F) vs. Latitude
    Humidity (%) vs. Latitude
    Cloudiness (%) vs. Latitude
    Wind Speed (mph) vs. Latitude

The script then further analyzes these relationships by running scatter plots with linear regressions, separated by Northern and Southern Hemispheres. 

    Northern Hemisphere - Temperature (F) vs. Latitude
    Southern Hemisphere - Temperature (F) vs. Latitude
    Northern Hemisphere - Humidity (%) vs. Latitude
    Southern Hemisphere - Humidity (%) vs. Latitude
    Northern Hemisphere - Cloudiness (%) vs. Latitude
    Southern Hemisphere - Cloudiness (%) vs. Latitude
    Northern Hemisphere - Wind Speed (mph) vs. Latitude
    Southern Hemisphere - Wind Speed (mph) vs. Latitude


VacationPy is a script that takes the data from WeatherPy and makes use of the Google Places API to provide analyses for a possible vacation. 

The script creates a heat map that displays the humidity for every city from WeatherPy, then narrows down the cities by ideal weather conditions: 

    A max temperature lower than 80 degrees but higher than 70
    Wind speed less than 7 mph
    Zero cloudiness
    Humidity less than 80%

It uses the Google Places API to find the first hotel for each "ideal" city located within 5000 meters of the coordinates and then plots the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
