# API-Challenge
---

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator to answer the question "What's the weather like as we approach the equator?". 

## Programming Language / Applications - Used for Analysis

  * Python 
    - Pandas Library
    - Matplotlib Library
    - Python APIs
    - JSON Traversals
  * Jupyter Notebook

## WeatherPy

### Analysis

Analysis includes each of the following in a [Jupyter Notebook](WeatherPy/WeatherPy.ipynb) with viewable Data Frames:

### Data Wrangling

Before beginning the analysis, checked the data for any city with Humidity greater than 100% and dropped them all. Used the cleaned data for the remaining steps.

### Data Visualization

* Generated a series of scatter plots to showcase the following relationships:

    - [Temperature (F) vs. Latitude](WeatherPy/output_data/lat_temp_scatter.png)
    - [Humidity (%) vs. Latitude](WeatherPy/output_data/lat_humidity_scatter.png)
    - [Cloudiness (%) vs. Latitude](WeatherPy/output_data/lat_cloudiness_scatter.png)
    - [Wind Speed (mph) vs. Latitude](WeatherPy/output_data/lat_wind_speed_scatter.png)

* Generated linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

    - [Northern Hemisphere - Temperature (F) vs. Latitude](WeatherPy/output_data/northern_hemisphere_lat_max_temp.png)
    - [Southern Hemisphere - Temperature (F) vs. Latitude](WeatherPy/output_data/southern_hemisphere_lat_max_temp.png)
    - [Northern Hemisphere - Humidity (%) vs. Latitude](WeatherPy/output_data/northern_hemisphere_lat_humidity.png)
    - [Southern Hemisphere - Humidity (%) vs. Latitude](WeatherPy/output_data/southern_hemisphere_lat_humidity.png)
    - [Northern Hemisphere - Cloudiness (%) vs. Latitude](WeatherPy/output_data/northern_hemisphere_lat_cloudiness.png)
    - [Southern Hemisphere - Cloudiness (%) vs. Latitude](WeatherPy/output_data/southern_hemisphere_lat_cloudiness.png)
    - [Northern Hemisphere - Wind Speed (mph) vs. Latitude](WeatherPy/output_data/northern_hemisphere_lat_windspeed.png)
    - [Southern Hemisphere - Wind Speed (mph) vs. Latitude](WeatherPy/output_data/southern_hemisphere_lat_windspeed.png)

### Data Analysis

Looked across all generated figures/plots and wrote down the observations or inferences that can be made from them. Included these observations below each plot/linear regression model in the notebook.

## VacationPy

### Analysis

Analysis includes each of the following in a [Jupyter Notebook](VacationPy/VacationPy.ipynb) with viewable Data Frames:

### Data Wrangling

Before beginning the analysis, checked the data for NaNs and dropped them all. Deleted unwanted columns. Converted the columns to appropriate data type. Used the cleaned data for the remaining steps.

### Data Visualization

* Generated a heat map that displays the humidity for every city

* Narrowed down the DataFrame to satisfy following ideal weather conditions:

    - A max temperature lower than 80 degrees but higher than 70
    - Wind speed less than 10 mph
    - Zero cloudiness

* Found the first hotel for each city located within 5000 meters using Google Places API

* Generated a map plotting the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

### Data Analysis

Looked across all generated figures/plots and wrote down the observations or inferences that can be made from them. Included these observations below each plot/linear regression model in the notebook.

---

## Contributors

- Usha Saravanakumar ([ushaakumaar](https://github.com/ushaakumaar))
