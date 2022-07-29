# Data-Science-Project-2-Stroke-Prediction-Model
Data Science Classification Project 

Author: Ryan Croasdale

Project Description 

For this Project I was tasked to find my own dataset that not only fit certain criteria, but also something that interests me or my future endeavors.

I chose a dataset that pertains to the healthcare industry. As I come from a pharmacy background, and would like to work in data science in the healthcare industry this dataset uncompases both these goals.

Context

According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths. This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.

Source of data

Kaggle: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset?resource=download

Methods

After cleaning the data and completing preprocessing. I used a Random Forest Classifier with Ada Boosting, Gradient Boosting, LightGBM and XGBoost tuning. I then used a KNN Model with SVC and Best K tuning. I then used a Log Reg Model with L1 and L2 tuning. I then tried a Decision Tree Classifier, and finally I used a Soft Voting Classifier Model.

I also tried using PCA with a KNN model to try to improve results.

Lastly I used feature engineering to combine two columns, using this new dataframe I once again used Random Forest Classifier with Gradient Boosting to see if my results would differ.

Results

All models tested performed very similiarly, with accuracy scores at or around 93.7%.

Therefore for my production model I will choose the Soft Voting Classifier Model, because it is an ensemble methat that combines that performances of multiple models to make predictions.

Soft Voting relies on the performance of multiple models, and such will not be hindered by large errors or misclassifications from one model. A poor performance from one model can be offset by a strong performance from other models.

The Soft Voting Classifier also performed well in precision and recall scores, which are indicitive that the model is performing and predicting correctly.

The data shows that if you're a 65+ y/o Male, Smoker, with Hypertension and Heart Disease with elevated Avg Glucose Level, has been married and had kids, and worked in the Private Sector then you would be an indivdual with the absolute highest risk to have a stroke.
