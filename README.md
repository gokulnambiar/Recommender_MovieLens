# MovieLens Recommender System

This project demonstrates the implementation of a recommender system using the **MovieLens 100k dataset**, developed and executed in **Databricks Community Edition**. The pipeline includes data extraction, exploratory data analysis (EDA), model training, and generating recommendations.

## Dataset
The **MovieLens 100k dataset** contains 100,000 ratings from 943 users on 1682 movies. Detailed information about the dataset is provided in the `readme` file within the "Data" folder, from the authors of the MovieLens 100k dataset.

## Pipeline Overview
1. **Data Extraction**:
   - Load the MovieLens dataset into Spark DataFrames.
2. **Exploratory Data Analysis (EDA)**:
   - Analyze user demographics, ratings distribution, genre preferences, and movie popularity.
3. **Model Training**:
   - Train a collaborative filtering model using ALS (Alternating Least Squares).
4. **Recommendation Generation**:
   - Generate personalized movie recommendations and identify popular movies in each genre.

## How to Run
1. Clone this repository.
2. Upload the dataset to Databricks.
3. Run the notebook `MovieRecommender.ipynb` in Databricks.
4. Review the results and visualizations.

## Dependencies
- **Apache Spark**
- **PySpark**
- **Matplotlib**
- **Pandas**

## Model Details
- **Algorithm**: Collaborative Filtering using ALS.
- **Features**:
  - Handles sparse datasets effectively.
  - Manages cold starts with a "drop" strategy for unseen users/items.
- **Evaluation Metric**: Root Mean Square Error (RMSE).
