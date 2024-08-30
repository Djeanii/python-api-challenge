# python-api-challenge
Overview
This project is part of a data analysis bootcamp where the goal is to utilize Python, APIs, and data visualization libraries to explore the relationship between weather variables and geographic location, as well as to identify ideal vacation spots based on specific weather conditions.

The challenge is divided into two main parts:

WeatherPy: Analyzes the weather of over 500 cities of varying distances from the equator to determine how weather changes as you approach the equator.
VacationPy: Identifies ideal vacation locations based on weather preferences and finds nearby hotels.
Part 1: WeatherPy
In the WeatherPy section, we:

Retrieve weather data for over 500 cities using the OpenWeatherMap API.

Generate scatter plots to visualize relationships between latitude and various weather parameters:
Temperature (°C)
Humidity (%)
Cloudiness (%)
Wind Speed (m/s)
Perform linear regression analysis to assess the strength of these relationships for both the Northern and Southern Hemispheres.

Key Findings
Temperature vs. Latitude: Strong correlation in both hemispheres; temperatures increase as you approach the equator.
Humidity, Cloudiness, and Wind Speed vs. Latitude: Weak correlations, indicating other factors beyond latitude influence these variables.

Part 2: VacationPy
In the VacationPy section, we:

Use the weather data to identify cities with ideal weather conditions for a vacation (e.g., moderate temperatures, low wind speeds, and clear skies).
Use the Geoapify API to find nearby hotels in these cities.
Visualize the results on a map, highlighting each city and its nearest hotel.

Installation
To run this project, you need to have Python installed along with the following libraries:

matplotlib
pandas
numpy
requests
scipy
hvplot
geoviews
cartopy (for geographic plots)

You will also need API keys for the OpenWeatherMap and Geoapify services. Place your keys in a file named api_keys.py as follows:
weather_api_key = "YOUR_OPENWEATHERMAP_API_KEY"
geoapify_key = "YOUR_GEOAPIFY_API_KEY"

Usage
1. Clone the repository
2. Install required libraries
3. You can install the required libraries using pip
4. Run the Notebooks- Open WeatherPy.ipynb and VacationPy.ipynb in Jupyter Notebook.

-Data Sources
OpenWeatherMap API: Provides current weather data for multiple cities.
Geoapify API: Used to find nearby hotels based on coordinates.

-File Structure
    -WeatherPy.ipynb: Notebook containing the analysis for Part 1.
    -VacationPy.ipynb: Notebook containing the analysis for Part 2.
    -output_data/cities.csv: CSV file containing the weather data for the analyzed cities.
    -output_data/Fig1.png to Fig4.png: Figures generated during the analysis.
    -api_keys.py: File containing the API keys (not included in the repository for security reasons).
    -.gitignore: Specifies files that should not be included in the repository (e.g., api_keys.py).

-Observations
There is a clear positive correlation between temperature and proximity to the equator (latitude close to 0).
Humidity, cloudiness, and wind speed show weak or no significant correlation with latitude, suggesting local geography and weather patterns play a more critical role.
Ideal vacation spots are scattered globally, and many are located near the coast, providing pleasant weather and tourist-friendly conditions.

License
This project is licensed under the MIT License - see the LICENSE file for details.
