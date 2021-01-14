# python-api-challenge: What's the Weather Like?

Background
Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
Now, we know what you may be thinking: "Duh. It gets hotter..."
But, if pressed, how would you prove it?

![image1](https://github.com/Auburn9698/python-api-challenge/blob/main/WeatherPy/Images/Globe.jpg)

# Part I - WeatherPy
In this exercise, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator utilizing a simple Python library and the OpenWeatherMap API to create a representative model of weather across world cities.

First, I created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude
[Image 1](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Lat_Temp.png)


Secondly, linear regression was run on each relationship, separating them into Northern and Southern Hemispheres.

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![Regression Image1](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Regression1.png)

![Regression Image2](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Regression2.png)

The next steps were:

* Randomly select at least 500 unique cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save a CSV of all retrieved data and a PNG image for each scatter plot.


# Part II - VacationPy

Next, I created a heat map that displays the humidity for each city.

![image2](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Heatmap.png)

The cities were narrowed down to those with ideal conditions.

![Ideal Cities Image](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Ideal_cities.png)

Using Google Places API , I found the first hotel for each city located within 5000 meters of your coordinates.


![image3](https://github.com/Auburn9698/python-api-challenge/blob/main/Images/Hotels_map.png)
