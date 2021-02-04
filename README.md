# Python API Homework - What's the Weather Like?

***Author: Michael Regpala  Date: 2/3/2021***

***Introduction***
As a data analyst i want to apply my new skills utilizng Python requests library to access API to return JSON data, which can be traversed and utilized in my notebook  This ia a very important skill to have as there is are many entities that make their data available for free or minimal cost, which can give our analsysis value.  After returning data we can utilize our new mapping and linear regression skills to identify correlations and data trends.


## WeatherPy Portion of homework
The jupyter notebook utilizes a function to return random cities based on the geo cordinate ranges and sample size parameters passed into the funtion in a dictionary object.  The funciton calls the citipy API, which will return the closest city to the random coordinates, creating a DataFrame of cities, which is saved as a csv file in the **output_data** directory for later use.  The OpenWather API is used to retrieve the weather stats and actual geo cooridnates for each of the cities selected randomly in newly created  DataFrame.  The following are links to the API's utilzied in WeatherPY notebook.
  - [citipy](https://pypi.pythoin.org/pyi/citipy)
  - [OpenWeatherMap API](https://openweathermap.org/api)

After the data has been loaded and contextulized the next step is to perform the following analysis:

***Create scatter plots to showcase the following relationships:***
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

*** Perform linear regression on each of the following relationships. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):***
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitud


### Part II - VacationPy
 Utilzing the csv file created by WeatherPY, a DataFrame is crreated, which will bew utilized to create a  heat map utilizng google maps API, which parameters are the city's location coordinates and coior intensity is the city's humidity.  

 The next step is to utilize Google Places API to pull in the first Hotel name returned located with 5000 meters of the city coordinates.  The last step is to create a layer on original heatmap with a in containing  **Hotel Name**, **City**, and **Country**.

***Runtime notes***
API keys are stored in the file **api_keys.py** in **api** directory.  The keys are set to blank, so you will need to update the file with your Google and OpenWeatherMap API keys.


