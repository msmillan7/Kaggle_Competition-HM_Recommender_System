# Kaggle Competition: H&M Recommender System

This project provides a solution for the H&M Recommender System chanllenge from Kaggle. The challenge consists of being able to predict what articles each customer will purchase in the 7-day period immediately after the training data ends. For so, Kaggle provides the purchase history of customers across time, along with supporting metadata. For further details, visit the competition's website below:

Link to the competition: https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations/overview

The solution we are providing to this challenge is a Rcommender System, consisting of two main phases: candidate generation via collaborative filtering and ranking using a LightGBM algorithm to predict the 12 items best suited for each customer.

The content of this repository is explained below:

Folders:
- /data: 
  -  Note: The original datasets provided by Kaggle (customers.csv, transactions.csv, articles.csv) are not included in this respository. Access to them is available through the link to the competition provided above.
  -  intermediate outputs generated during the execution of the pipelines.
  -  /subs: Contains the final submission files (output of the model in the requested format).
  
-  /Rough Code: Contains rough notebooks and files used during the development of the project.

- root: Contains the four final pipelines of the project. 
  -  00_EDA.ipynb: Exploratory Data Analysis of the training data.
  -  01_preprocessing.ipynb: Memory reducing, data cleaning, data subsetting and generation of training and validation datasets.
  -  02_collaborative-filtering.ipynb: Candidate Generation phase. Selection of potential relevan items via Collaborative Filtering.
  -  03_ranking.ipynb: Ranking phase using a LightGBM algorithm to predict the final 12 items for each customer.
