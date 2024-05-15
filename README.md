Introduction
The objective of this project is to develop a machine learning model that can suggest appropriate listing prices for Airbnb properties in Antwerp, Belgium, based on various features from the dataset. The goal is to assist property owners in setting competitive and fair prices.

Dataset
The dataset consists of the following tables:

Calendar: Contains listing dates, availability, and prices.
Listings: Contains details about each property.
Hosts: Contains information about the hosts.
Reviews: Contains reviews and comments about the listings.
Data Understanding
Initial Exploration
Calendar table: 319,192 entries, 1,749 unique listings
Listings table: 1,749 entries
Hosts table: 1,111 entries
Reviews table: 62,987 entries
Key Findings
The dataset contains information on availability, prices, property details, host details, and reviews.
Missing values and data anomalies were identified and handled.
Data Cleaning and Preprocessing
Handling Missing Values
Missing values in critical columns like price were addressed.
Imputation strategies were used for other missing values.
Feature Engineering
Extracted year and month from the date column.
Created new features based on the available data.
Exploratory Data Analysis
Visualizations and Correlations
Scatter plots for bedrooms, beds, and accommodates vs. price.
Correlation analysis revealed key predictors: latitude, longitude, review_count, bedrooms, and beds.
Key Insights
Location and review count significantly impact listing prices.
Larger properties with more bedrooms and beds tend to have higher prices.
Modeling and Evaluation
Model Selection and Training
Models trained: Linear Regression, Decision Tree Regressor, Random Forest Regressor, Gradient Boosting Regressor.
Evaluation based on Mean Absolute Error (MAE).
Evaluation Metrics
Random Forest Regressor had the best performance with an MAE of 11.84 on the test set.
Feature Importance
Top predictors: latitude, longitude, review_count, bedrooms, and beds.
Key Findings
Geographic location and review count are crucial in determining listing prices.
The Random Forest Regressor is effective in predicting listing prices.
Recommendations
Use location and review count data to optimize pricing strategies.
Focus on increasing the number of reviews for better price optimization.
How to Run
Clone the Repository
bash
Copy code
git clone <repository-url>
Navigate to the Project Directory
bash
Copy code
cd airbnb-price-prediction
Install the Required Packages
bash
Copy code
pip install -r requirements.txt
Run the Notebooks
bash
Copy code
jupyter notebook
Notebooks
Data Understanding: Explore the structure and content of the dataset.
Data Cleaning and Preprocessing: Handle missing values and perform feature engineering.
Exploratory Data Analysis: Visualize relationships and compute correlations.
Modeling and Evaluation: Train and evaluate different regression models.
Key Findings
Geographic location and review count significantly impact listing prices.
The Random Forest Regressor is effective in predicting listing prices with a Mean Absolute Error (MAE) of 11.84 on the test set.
Recommendations
Use location and review count data to optimize pricing strategies.
Focus on increasing the number of reviews for better price optimization.
