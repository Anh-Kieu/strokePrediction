## CSCI 349 Final Project: Modelling Stroke With Patient's Medical Condition ##
### Anh Kieu - Rafe Batchelor ###
#### drive url for video: https://drive.google.com/file/d/1qF9Te-tRMUcBYEiYbj1xyvkqdWKDqRP_/view?usp=sharing ####
#### link to slides: https://docs.google.com/presentation/d/1uEplmlos0AesmlXRaem-ERqejRQY1ej5UflHpI-o4oM/edit?usp=sharing ####

 With the Stroke Prediction Dataset from Kaggle, we want to understand more about stroke and its likelihood on a patient. \
Firstly, we analyzed and made visualization for the features in the dataset, exploring the relationship between medical attributes and stroke tendency. We concluded that most of the attributes, except gender and residence type, are related to stroke likelihood. We use KNN Imputer for missing bmi values, based on age and average glucose level. \
Then, we continued to build model trying to predict stroke likelihood with Decision Tree, Random Forest and Logistic Regression. We first upsample the dataset to avoid imbalance using SMOTE, then tuning the models with grid search. 
We found out that most models are comparable with regard to performance. Since we use recall for class 1 as our main scoring, we decide that Random Forest performed the best out of the three models. \
We think that with more time, we can make the following improvements to make our results more desirable:
- Smaller sample of the dataset (remove unrelated attributes)
- Different variations of SMOTE or imbalance sampling method (RandomOverSample)
- More models (i.e XGBoost, AdaBoost, simple ANN) + bigger range of parameters
