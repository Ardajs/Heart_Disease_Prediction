# Heart_Disease_Prediction
Heart disease prediction using a Random Forest classifier based on clinical health indicators with feature importance analysis and model evaluation.


## Heart Disease Prediction using Random Forest

This project aims to predict the presence of heart disease using machine learning techniques. A Random Forest classifier was applied to analyze clinical health indicators and classify whether a patient has heart disease or not. The project demonstrates how machine learning models can assist in analyzing medical datasets and identifying patterns related to cardiovascular diseases.

## Dataset

The dataset used in this project contains several clinical attributes commonly used in cardiovascular disease diagnosis.

Features included in the dataset:

Age

Sex

Chest Pain Type

Blood Pressure (BP)

Cholesterol

Fasting Blood Sugar (FBS over 120)

EKG Results

Maximum Heart Rate (Max HR)

Exercise Induced Angina

ST Depression

Slope of ST

Number of Vessels (Fluoroscopy)

Thallium Test Result

Target variable:

Presence → Heart disease detected

Absence → No heart disease

## Methodology

The following steps were applied during the machine learning workflow:

Data loading and preprocessing

Converting the target variable into numerical values

Splitting the dataset into training and testing sets

Training a Random Forest classifier

Evaluating the model using classification metrics

Analyzing feature importance to understand model behavior

Libraries used in the project include:

pandas

numpy

scikit-learn

matplotlib

## Model

The machine learning model used in this project is the Random Forest Classifier, which is an ensemble learning method that combines multiple decision trees to improve prediction performance and reduce overfitting.

Example model parameters used:

n_estimators = 200

max_depth = 5

random_state = 42

Random Forest was chosen because it performs well on tabular datasets and provides feature importance analysis, which helps interpret the model's decisions.

## Model Performance

The trained model achieved the following performance on the test dataset:

Accuracy: 87%

Classification metrics indicate that the model performs well in identifying healthy individuals while also detecting most heart disease cases.

Confusion Matrix:

31 healthy patients correctly classified
16 heart disease cases correctly detected
5 disease cases missed
2 healthy patients incorrectly classified as diseased

These results show that the model captures meaningful patterns in the data, although some disease cases remain difficult to detect.

## Feature Importance Analysis

Feature importance analysis was performed to understand which variables have the strongest influence on the model’s predictions.

The most important features identified by the model include:

Thallium Test Result

ST Depression

Chest Pain Type

Maximum Heart Rate

Number of Vessels

These features are clinically relevant indicators commonly used in cardiovascular diagnostics.

Lower importance features include:

Fasting Blood Sugar

EKG Results

Sex

This suggests that the model relies more heavily on clinical test results rather than demographic variables when predicting heart disease.
