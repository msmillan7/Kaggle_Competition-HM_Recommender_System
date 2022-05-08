# Kaggle_Competition-HM_Recommender_System
https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations/overview

Kaggle Challenge: For this challenge you are given the purchase history of customers across time, along with supporting metadata. Your challenge is to predict what articles each customer will purchase in the 7-day period immediately after the training data ends. Customer who did not make any purchase during that time are excluded from the scoring.

Works with the parquets generated from 01_processing from commit "integrate collab_filter results into ranking pipeline: e79720d8cfd7ecdf49894be75755f5eb134ad8c8":

* articles_sample_gt0transactions.parquet  
* customers_sample_gt0transactions.parquet  
* transactions_train_sample_gt0transactions.parquet  
* customers_recommended_articles.csv  
* val_ground_truth.pkl  