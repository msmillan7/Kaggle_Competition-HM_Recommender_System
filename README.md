# Kaggle_Competition-HM_Recommender_System
https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations/overview

Kaggle Challenge: For this challenge you are given the purchase history of customers across time, along with supporting metadata. Your challenge is to predict what articles each customer will purchase in the 7-day period immediately after the training data ends. Customer who did not make any purchase during that time are excluded from the scoring.

1. Created a train/ validation split in 01_processing. Both train and validation sets are subsets/ samples obtained by taking 5% of the customers (the customers in validation are the same as those in training). NOTE: We did not subset by MIN_TRANSACTIONS because it would have complicated the train/ val split. 
2. Works with the parquets generated from 01_processing explained in (1)

* transactions_train_sample_gt0transactions.parquet  
* customers_train_sample_gt0transactions.parquet  
* articles_train_sample_gt0transactions
* transactions_val_sample_gt0transactions.parquet
* articles_val_sample_gt0transactions.parquet  
* customers_recommended_articles.csv  
* val_ground_truth.pkl  