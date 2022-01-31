# python-api-challenge
Using Open Weather and Google Maps APIs and JSON to access and analyze weather data to examine how weather may change as one approaches the equator.


## **WeatherPy**
A list of >500 cities was created based on randomly generated longitude and latitude. Data for location coordinates, max temperature, humidity, cloudiness, wind speed, country, and date of access was extracted and analyzed to examine trends based on distance from the equator. Scatterplots were created to examine how latitude (distance from the equator) effects max temperature, humidity, cloudiness, and wind speed. Linear regressions were performed for these parameters for cities both in the northern and southern hemispheres and correlation coefficients were calculated. 

### **Observations based on the data analysis** 
The graphs and linear regressions revealed that the strongest correlation to distance from the equator was with the maximum temperature for cities in the northern hemisphere - the further away from the equator, the lower the maximum temperature is likely to be. Interestingly, based on the data, there was no correlation for cities in the southern hemisphere.

Cloudiness of a city did not have any correlation to distance from the equator. Cloudiness, in the northern cities particularly, visually appeared to have the most even distribution across the plot.

Wind speed also did not have any correlation to distance from the equator. Wind speed for the majority of northern cities was below 15 mph, while southern cities largely had a wind speed below 10 mph. 


## **VacationPy**
This section used the data gathered from WeatherPy as well as the jupyter-gmaps and the Google Places API to determine the best vacation cities based on weather. The humidity of the cities in the data set was mapped in a heatmap. Ideal vacation conditions were defined (max temperature between 68 and 80 degrees Fahrenheit, wind speed less than 10 mph, and no clouds!) and cities that matched those conditions were identified. Hotel data for these cities was retrieved using Google Places API and these were mapped on top of the heatmap. 


