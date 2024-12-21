# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
My project aims to explore the relationship between bike station availability and Yelp point-of-interest (POI) characteristics to inform urban planning decisions. My primary goal was to understand how POI features, such as ratings and geographic locations, correlate with bike station metrics, allowing for data-driven recommendations for optimizing bike station placements across a city. 

## Process
1. Data Collection:
   - Gathered data on bike station availability and Yelp POI data. Created datasets `stations_Monaco_df` and `yelp_df`.

2. Data Cleaning and Preprocessing:
   - Verified and cleaned latitude/longitude values.
   - Merged datasets by calculating geospatial distances to link bike stations to nearby Yelp POIs.

3. Exploratory Data Analysis (EDA):
   - Investigated trends between Yelp POI characteristics (e.g., ratings, categories) and bike station metrics.
   - Created visualizations, including scatter plots and boxplots, to analyze geospatial distributions and POI ratings.

4. Model Building:
   - Developed an Ordinary Least Squares (OLS) regression model to quantify the impact of POI characteristics (ratings, latitude, longitude) on bike station availability.

5. Insights & Recommendations:
   - Interpreted model results to derive actionable insights for urban planning and business developers.



## Results
- Comparative Quality of API Coverage:
   - POI restaurant categories such as "Italian" and "Indian" displayed higher average Yelp ratings compared to others. This tells us that italian and indian cuisine seems to be most popular in Monaco, while Cafes and Japanese cuisine seem to be the least popular. This is helpful for business developers as it signifies what kind of restaurants will be popular and more likely to be successful. This information also tells you that you where the area might be liking, like in Japanese cuisine, and that might drive the demand or need for a Japanese restaurant in the area.
   - Geospatial analysis revealed that high-rated POIs tend to cluster near certain bike stations. Regions with high-rated POIs tend to have better bike station accessibility, suggesting a potential strategy for optimizing bike network coverage.
- Regression Model:
   - R-squared: 0.110, indicating a modest fit.
   - Latitude and longitude significantly influenced bike availability:
     - Latitude: Positive correlation with bike availability.
     - Longitude: Negative correlation with bike availability.
     - Yelp ratings were not statistically significant in predicting bike availability.

## Challenges 
1. Data Integration:
   - Merging datasets required custom geospatial calculations to link bike stations and Yelp POIs.
2. Sparse Features:
   - The model's explanatory power was limited due to the absence of factors like foot traffic and time-of-day trends.
3. Technical Issues:
   - Encountered delays from software installation errors, including module incompatibilities with `matplotlib` and `statsmodels`. Also difficulties with using the API keys. 
## Future Goals
1. Additional Features:
   - Incorporate metrics like foot traffic, POI density, and business hours for deeper insights.
2. Enhanced Modeling:
   - Experiment with machine learning models (e.g., Random Forests) to improve prediction accuracy.
3. Time-Series Analysis:
   - Explore temporal trends in bike availability and its relationship with POI characteristics.