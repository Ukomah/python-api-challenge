# Python API Challenge

## Project Overview

The Python API Challenge is a comprehensive exploration of weather patterns and their relationship with latitude. Leveraging Python's capabilities in handling requests, working with APIs, and navigating JSON data, this project addresses a fundamental question: "What is the weather like as we approach the equator?"

## WeatherPy - Exploring Weather Variables

### Objectives
1. **Retrieve Weather Data**: Utilize the citipy Python library and the OpenWeatherMap API to gather weather data for over 500 cities around the world.
2. **Visualize Relationships**: Generate scatter plots showcasing the relationships between latitude and various weather variables, including temperature, humidity, cloudiness, and wind speed.
3. **Linear Regression Analysis**: Compute linear regression for each relationship, differentiating between the Northern and Southern Hemispheres.

### Findings
#### Temperature vs. Latitude
- **Northern Hemisphere:**
  - There is a robust positive correlation between latitude and temperature.
  - The R-squared Value of 0.78 indicates a strong linear relationship, suggesting that the model is a good fit for the data.
  - The positive slope (0.74) implies that as latitude increases (moving towards the North Pole), the temperature tends to rise.
  - The intercept (35.92) signifies the baseline temperature at the equator (latitude = 0).
- **Southern Hemisphere:**
  - Positive correlation exists, but it's weaker (R-squared Value: 0.40).
  - The positive slope (0.32) indicates an increasing trend as latitude increases (moving towards the South Pole).
  - The intercept (29.09) implies the baseline temperature at the equator.

#### Humidity vs. Latitude
- **Northern Hemisphere:**
  - There is a weak positive linear relationship between latitude and humidity.
  - The R-squared Value of 0.14 suggests a relatively weak correlation, indicating that latitude alone might not be a strong predictor of humidity.
  - The positive slope (0.43) implies a slight tendency for humidity to increase as latitude increases.
  - The intercept (58.06) indicates the baseline humidity at the equator.
- **Southern Hemisphere:**
  - Weak positive linear relationship (R-squared Value: 0.08).
  - The positive slope (0.38) suggests a subtle increase in humidity with higher latitudes.
  - The intercept (80.83) indicates the baseline humidity at the equator in the Southern Hemisphere.

#### Cloudiness vs. Latitude
- **Northern Hemisphere:**
  - Latitude has limited predictive power for cloudiness (R-squared Value: 0.07).
  - The positive slope (0.53) indicates a slight increase in cloudiness with rising latitude.
  - The model's fit appears limited, suggesting latitude alone may not be a reliable predictor.
- **Southern Hemisphere:**
  - Limited predictive power for cloudiness (R-squared Value: 0.07).
  - The positive slope (0.65) suggests a minor increase in cloudiness with higher latitudes.
  - Similar to the Northern Hemisphere, the model's capacity to predict cloudiness appears constrained.

#### Wind Speed vs. Latitude
- **Northern Hemisphere:**
  - Latitude alone is not highly effective in predicting wind speed (R-squared Value: 0.01).
  - The relatively low R-squared value suggests a weak linear relationship between latitude and wind speed.
  - The negative slope (-0.01) indicates a subtle decrease in wind speed as latitude increases.
  - The intercept (3.65) implies the baseline wind speed at the equator.
- **Southern Hemisphere:**
  - Weak linear relationship (R-squared Value: 0.09).
  - The negative slope (-0.06) suggests a subtle decrease in wind speed as latitude increases.
  - Other meteorological and geographical factors likely play a more substantial role in influencing wind speed levels.

## VacationPy - Planning Future Vacations

### Objectives
1. **Mapping Cities**: Use Jupyter notebooks, the geoViews Python library, and the Geoapify API to map cities and display humidity levels.
2. **Ideal Weather Conditions**: Narrow down city selections based on specified weather conditions (temperature, wind speed, cloudiness).
3. **Finding Nearby Hotels**: Utilize the Geoapify API to identify the nearest hotel within 10,000 meters of each city.

### Findings
- Starting searches for cities like Sur and Cabo San Lucas have identified hotels nearby, while others may not yield results.

## File Structure

The project is organized into two main parts:

- **WeatherPy:**
  - Contains the Jupyter notebook (`WeatherPy.ipynb`) for weather analysis.
  - Utilizes a separate Python script (`api_keys.py`) to store API keys securely.
  
- **VacationPy:**
  - Includes the Jupyter notebook (`VacationPy.ipynb`) for vacation planning.
  - Incorporates a structured file (`hotel_df`) to store information about hotels and cities.

## Real-World Data Analysis

This project is an academic exercise assigned by the University of Toronto, involving the practical application of data analytics skills to real-world data. By exploring the relationships between weather variables and latitude, we gain valuable insights into the complexities of weather patterns across different geographical zones.

Feel free to explore the Jupyter notebooks (`WeatherPy.ipynb` and `VacationPy.ipynb`) for a detailed walkthrough of the analyses and findings.
