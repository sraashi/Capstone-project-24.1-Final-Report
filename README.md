# Capstone-project-24.1-Final-Report
Capstone project - Final

Problem Statement: The main objective here to be able to predict how a compound may perform against a target using a set of available data. 
Drug discovery requires the screening of many 1000s of molecules to arrive at potent compounds that perform well amongst many parameters so I see a lot of potential where AI/ML can help increase efficiency here.
 

Model Outcomes or Predictions: Using a regression algorithm, the potencies of compounds can be predicted. Using a classification model, compounds can be classified as active or inactive based on a cut-off value. 
Supervised model will be used where a training set will be used to train the model followed by predictions on a test set. 


Data Acquisition: Here, the data will be Physico-chemical data and 2D structure of compounds publicly available. 
The BACE dataset provides quantitative (IC50) and qualitative (binary label) binding results for a set of inhibitors of human β-secretase 1 (BACE-1). All data are experimental values reported in scientific literature over the past decade, some with detailed crystal structures available. A collection of 1522 compounds with their 2D structures and properties are provided.
Dataset from this paper - "Computational Modeling of β‐Secretase 1 (BACE-1) Inhibitors Using Ligand Based Approaches". Govind Subramanian, Bharat Ramsundar, Vijay Pande, Raja Aldrin Denny

Data Preprocessing/Preparation:
Assess the dataset using describe and info
Check for missing values using isna() and sum()
Remove any duplicates and columns that have unique values
Check for distribution of the data and skewing of the potency values 
Split the data into 33% test set and 66% training set

Modeling: The models I tested on this dataset were Logistic regression, KNN, SVC, Linear regression with polynomial features


Model Evaluation:

