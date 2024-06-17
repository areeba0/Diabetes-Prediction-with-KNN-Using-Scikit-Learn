# Scikit-Learn Implementation of KNN for Diabetes Risk Prediction
This code implements a K-Nearest Neighbors (KNN) classifier to predict the onset of diabetes based on several medical predictors. The dataset used for this analysis is sourced from the Pima Indians Diabetes Database. This project includes data preprocessing, the implementation of a custom KNN classifier, model evaluation, and visualization of results.

# Dependencies
- numpy - Numerical computing library.
- pandas - Data manipulation and analysis library.
- scikit-learn - Machine learning library for Python.
- matplotlib - Plotting library.
- seaborn - Data visualization library.

# Implementation Details

## 1. Data Preprocessing
- Handling Zero Values:
Columns Glucose, BloodPressure, SkinThickness, BMI, and Insulin are not allowed to have zero values. Zeros are replaced with the mean value of the column.
- Train-Test Split:
The data is split into training and testing sets using an 80-20 split.

## 2.KNN Classifier
- Euclidean Distance Calculation:
A custom function calculates the Euclidean distance between instances.
- Prediction:
For each test instance, the K nearest neighbors are found, and the majority class among these neighbors is used as the predicted label.

## 3.Accuracy Evaluation
* The accuracy of the classifier is computed for different values of k (3, 5, 11).

## 4. Visualization
- Accuracy Plot: Accuracy vs. k values.
- Scatter Plot: Visualization of Glucose vs. BloodPressure for the test set, with different colors indicating the class.

# Dataset
The dataset is the Pima Indians Diabetes Database. It contains medical records for women of Pima Indian heritage, aged 21 and older. The data includes 8 features and a target variable indicating diabetes.
## Features:
- Pregnancies: Number of times pregnant
- Glucose: Plasma glucose concentration (2 hours in an oral glucose tolerance test)
- BloodPressure: Diastolic blood pressure (mm Hg)
- SkinThickness: Triceps skinfold thickness (mm)
- Insulin: 2-Hour serum insulin (mu U/ml)
- BMI: Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction: Diabetes pedigree function
- Age: Age (years)
## Target:
- Outcome: Class variable (0 or 1), 268 of 768 are 1, the others are 0
