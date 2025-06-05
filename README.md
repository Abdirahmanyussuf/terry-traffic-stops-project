Terry Traffic Stops – Contraband Prediction
 Project Overview
This project aims to build a predictive model to determine whether contraband was found during a traffic stop. The goal is to assist law enforcement analysis by identifying patterns in stop outcomes using machine learning.

Dataset Description
The dataset is based on traffic stop records and includes features such as:

Stop Resolution

Weapon Type

Officer and Subject Demographics

Call Types

Flags (Arrest, Frisk)

Officer Age

Target: contraband_found (1 if contraband was found, else 0)

 Data Preprocessing
Checked and confirmed correct data types

Handled class imbalance using class_weight='balanced'

Categorical features encoded using OneHotEncoder via a ColumnTransformer

Train-test split (80/20) with stratification to maintain class distribution

No duplicates in train or test sets

Modeling Approach
Model: Logistic Regression

Pipeline used for clean preprocessing and model training

Balanced class weights to handle class imbalance

Used max_iter=500 to ensure convergence

 Evaluation Metrics
Evaluated on test data using:

Accuracy

Precision

Recall

F1 Score

Confusion Matrix

 All metrics reported a perfect score (1.0), indicating either a very strong model or potential overfitting.

 Tech Stack
Python

Pandas, NumPy

Scikit-learn

