# Python API Homework - What's the Weather Like?

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?


## Part I - WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

Your first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot add a sentence or too explaining what the code is and analyzing.

Your second requirement is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* [Northern Hemisphere - Temperature (F) vs. Latitude](WeatherPy/Images/city_latitude_vs_max_temp-Northern_Hemisphere.png)
* [Southern Hemisphere - Temperature (F) vs. Latitude](WeatherPy/Images/city_latitude_vs_max_temp-Southern_Hemisphere.png)
* [Northern Hemisphere - Humidity (%) vs. Latitude](WeatherPy/Images/city_latitude_vs_humidity-Northern_Hemisphere.png)
* [Southern Hemisphere - Humidity (%) vs. Latitude](WeatherPy/Images/city_latitude_vs_humidity-Southern_Hemisphere.png)
* [Northern Hemisphere - Cloudiness (%) vs. Latitude](WeatherPy/Images/city_latitude_vs_cloudiness-Northern_Hemisphere.png)
* [Southern Hemisphere - Cloudiness (%) vs. Latitude](WeatherPy/Images/city_latitude_vs_cloudiness-Southern_Hemisphere.png)
* [Northern Hemisphere - Wind Speed (mph) vs. Latitude](WeatherPy/Images/city_latitude_vs_windspeed-Northern_Hemisphere.png)
* [Southern Hemisphere - Wind Speed (mph) vs. Latitude](WeatherPy/Images/city_latitude_vs_windspeed-Southern_Hemisphere.png)

After each pair of plots explain what the linear regression is modeling such as any relationships you notice and any other analysis you may have.

Your final notebook must:

* Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save a CSV of all retrieved data and a PNG image for each scatter plot.