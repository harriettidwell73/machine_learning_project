Mall Customer Segmentation (Unsupervised Learning Project)

Project Overview

This project applies unsupervised machine learning to segment mall customers based on their demographic and behavioral patterns. Using the classic Mall Customers dataset, the goal was to identify meaningful customer groups that could support marketing strategy, targeted promotions, and business insights.
The workflow includes data cleaning, preprocessing, normalization, clustering, and demographic interpretation. The final output is a set of five customer segments derived using K Means clustering, supported by visualizations and cluster level summaries.

Tools & Technologies Used

  •	Python 3.x

  •	Pandas — data loading, cleaning, and manipulation

  •	NumPy — numerical operations

  •	Matplotlib — visualizations (Elbow plot, cluster scatterplot)

  •	Scikit Learn

    o	StandardScaler for z score normalization

    o	KMeans for clustering

  •	Jupyter Notebook — interactive development and documentation

Dataset Used

Mall Customers Dataset (200 rows × 5 columns) Includes:

  •	CustomerID — unique identifier

  •	Gender — Male/Female

  •	Age — customer age

  •	Income — annual income (cleaned from string format to numeric)

  •	SpendingScore — mall assigned score (1–100)
This dataset is widely used for introductory clustering exercises because it contains both demographic and behavioral variables that naturally form distinct groups.

Methods & Workflow

1. Data Cleaning & Preprocessing
  •	Removed commas and “USD” from the Income column
  •	Converted income values to numeric
  •	Selected relevant features: Income, SpendingScore, Gender, Age
  •	Applied z score normalization to numeric features

2. Elbow Method
  •	Computed Within Cluster Sum of Squares (WSS) for k = 1–10
  •	Identified k = 5 as the optimal number of clusters

3. K Means Clustering
  •	Fit K Means with n_clusters = 5
  •	Visualized clusters using scaled income and spending score
  •	Extracted cluster centers for interpretation

4. Demographic Interpretation
Using gender distribution and average age per cluster, each group was assigned a descriptive name such as:
  •	Occasional Visitors
  •	Premium Loyalists
  •	Value Seeking Enthusiasts
  •	High Income Minimalists
  •	Budget Shoppers

Skills Demonstrated

  •	Data cleaning and preprocessing

  •	Feature selection and normalization

  •	Exploratory data analysis (EDA)

  •	Unsupervised learning with K Means

  •	Cluster evaluation and interpretation

  •	Visualization of machine learning results

  •	Clear documentation and reproducible workflow
