# Project 2: Prediction of Sale Price

In this project, we were provided the Ames Housing dataset and tasked to create a model to predict the sale price via the regression technique. The objective of the project is to perform iterative improvements to the model to achieve a better prediction result. The [data description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt) is provided in the link

The project is split into 5 notebooks:

- First notebook cleaning of data and filling of null values
- Second Notebook exploratory data analysis and feature engineering
- Third Notebook exploratory data analysis, feature engineering and modelling
- Fourth Notebook is second iteration of exploratory data analysis, feature engineering and modelling to improve the model
- Fifth Notebook is third iteration of exploratory data analysis, feature engineering and modelling to improve the model

# Problem Statement

From the Ames Housing dataset, create a model to predict the sale price and perform improvements to the model after it is created

# Executive Summary

The Ames Housing dataset consists of 81 features and 2051 rows. Included in the features are various characteristics of the property that was sold and their respective sale price. 

In this project, an agile methodology was adopted, for 3 iterations. We performed cleaning to the dataset, performed exploratory data analysis, feature engineering and create a model to predict the sale price of the test data set which we do not know the price.

After the data is cleaned, exploratory data analysis was performed through the dataset and also Kaggle's data dictionary to determine the best way to fill up missing values and determine which rows or features should be dropped.

The first model was created, selecting the top features which has the highest correlation with the sale price of the test dataset was predicted. From the first iteration, we are able to determine which features are highly correlated to the sale price and thus able to streamline the features to be utilised.

In the second iteration, cleaning was performed again, and interaction features was manually created based on understanding of how similar features of the property can be grouped together as an interaction. A correlation heatmap was plotted and 9 features which has the highest correlation to sale price was selected. The model was fitted with Ridge, sale price was predicted and submitted to Kaggle. The public score from Kaggle's submission is 30, 596 and the private score 34,528

In the third iteration, Polynomial Features was performed on the 9 features and the heatmap was plotted again. A total of 6 features was selected and fitted with Ridge. The sale price was predicted and submitted to Kaggle. The public score from Kaggle's submission is 26,639 and private score is 39,360.

# Conclusion

Open sources indicate that for this competition, Kaggle calculate the public score from 30% of the test dataset and the private score is calculated from 70% of the dataset. Although the second model shows that there is an improvement in the public score, the private score saw a decrease in performance. It is decided that the first model is better amongst the two as it displayed less discrepencies between their private and public score.