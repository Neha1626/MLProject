# MLProject
Bangalore-house's-rate
This notebook is for people who are looking to buy a place in Bangalore city(INDIA)
Created a model that predicts Bangalore house rate to help people to know about the prices of house in various places without the need of contacting different agents for the same.
Data was collected from Kaggle
Data shape is 13320 rows and 9 columns.
# EDA
Column 'total_sqft' was provided in avergare terms i.e 1195 - 1440, converted the same to float by taking the average of the numbers.

Created a new column - 'price_per_sqft' for better analysis.

Scaled down the number of locations to 241 from 1287 since most of the location occured less than 10 times.

On an average, the ratio between total_sqrt_foot and number of BHK should always be 300, hence we removed all the entries with values lesser than 300.
# ML MODEL
Performed One hot encoding to represent the categorical values in binary form since machine learning algorithms cannot operate on label data directly.
# Predictions
Built a function to predict the house price with location, number of Square foot area, Bathroom, and BHK
