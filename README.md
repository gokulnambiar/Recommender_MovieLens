MovieLens Recommender System

Description:
This project demonstrates the implementation of a recommender system using the MovieLens 100k dataset, developed and executed in Databricks Community Edition. The pipeline includes data extraction, exploratory data analysis (EDA), model training, and generating recommendations.


Dataset:
The MovieLens 100k dataset is used in this project. It contains 100,000 ratings from 943 users on 1682 movies. Specifics of the dataset detailed in readme file within the "Data" folder, from the authors.


Pipeline Overview:
Data Extraction: Load the MovieLens dataset into Spark DataFrames.
Exploratory Data Analysis (EDA): Analyze user demographics, ratings distribution, genre preferences, and movie popularity.
Model Training: Train a collaborative filtering model using ALS (Alternating Least Squares).
Recommendation Generation: Generate personalized movie recommendations for users and identify popular movies in each genre.


Steps
1. Data Extraction
2. Exploratory Data Analysis (EDA)
3. Model Training
4. Recommendation Generation


How to Run
Clone this repository.
Upload the dataset to Databricks.
Run the notebook MovieRecommender.ipynb in Databricks.
Review the results and visualizations.


Dependencies:
Apache Spark
PySpark
Matplotlib
Pandas


Model Details:
Algorithm - Collaborative Filtering using ALS.
Features -
  Handles sparse datasets effectively.
  Accounts for cold starts with a "drop" strategy for unseen users/items.
Evaluation Metric - Root Mean Square Error (RMSE).
