# Capstone-project-24.1-Final-Report
Capstone project - Final

Problem Statement: The main objective here to be able to predict how a compound may perform against a target using a set of available data. 
Drug discovery requires the screening of many 1000s of molecules to arrive at potent compounds that perform well amongst many parameters so I see a lot of potential where AI/ML can help increase efficiency here.
 

Model Outcomes or Predictions: Using a regression algorithm, the potencies of compounds can be predicted. Using a classification model, compounds can be classified as active or inactive based on a cut-off value. 
Supervised models will be used for oth classification and regression. 


Data Acquisition: Here, the data will be Physico-chemical data and 2D structure of compounds publicly available. 
The BACE dataset provides quantitative (IC50) and qualitative (binary label) binding results for a set of inhibitors of human β-secretase 1 (BACE-1). All data are experimental values reported in scientific literature over the past decade, some with detailed crystal structures available. A collection of 1522 compounds with their 2D structures and properties are provided.
Dataset from this paper - "Computational Modeling of β‐Secretase 1 (BACE-1) Inhibitors Using Ligand Based Approaches". Govind Subramanian, Bharat Ramsundar, Vijay Pande, Raja Aldrin Denny

Data Preprocessing/Preparation:
Assess the dataset using describe and info
Check for missing values and remove any data that is missing
Remove any duplicates and columns that have unique values
Check for distribution of the data and skewing of the potency values 
Split the data into 33% test set and 66% training set
Pairwise correlation plots between datasets showed how the data varies acorss variables
I tried dimensionality reduction with PCA but the variance was low, so would need to evaluate which features contribute to the variance and re-assess. 

Modeling and model evaluation: The classification models I tested on this dataset were Logistic regression, KNN, SVC and assessed the models for accuracy, sensitivity, specificity and F1_scores. 
Between the 3 models, SVC had the highest score for the test set with a high sensitivity and specificity but logistic regression had the highest F1_score taking into account precision and recall and hence, that might be the best model to go with for classification. 

I also performed ridge regression and linear regression with polynomial features on this dataset to predict the pIC50 values with the R2 score being quite low, and hence can be improved. 

Next steps to try and improve the model:
Re-evaluate PCA with select features
I have not tried ensemble techniques such as random forest and boosted and could be used to improve the modeling
Could also use permutation importance for feature selection. 

