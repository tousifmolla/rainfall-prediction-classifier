# Rainfall Prediction Classifier

A machine learning classification project that predicts rainfall using historical Australian weather data.

The project compares Random Forest Classifier and Logistic Regression models using a complete Scikit-learn machine learning pipeline, including preprocessing, hyperparameter tuning, prediction, evaluation, and feature importance analysis.

## Project Objective

The objective is to build a classification model capable of predicting whether it will rain based on historical weather observations.

The project demonstrates an end-to-end machine learning workflow, from data preparation to model comparison.

## Dataset

The project uses Australian weather observations containing features such as:

- Temperature
- Humidity
- Atmospheric pressure
- Rainfall
- Sunshine
- Evaporation
- Wind speed
- Wind direction
- Cloud cover
- Location
- Previous rainfall information
- Season

The target variable represents whether rainfall occurs.

## Machine Learning Workflow

The project includes:

1. Data loading and cleaning
2. Missing-value handling
3. Feature engineering
4. Train/test splitting
5. Numerical feature standardization
6. Categorical feature one-hot encoding
7. Scikit-learn Pipeline and ColumnTransformer
8. Random Forest classification
9. Logistic Regression classification
10. Hyperparameter tuning with GridSearchCV
11. Model evaluation
12. Confusion matrix analysis
13. Classification report analysis
14. Feature importance analysis

## Models

### Random Forest Classifier

Random Forest was trained and optimized using GridSearchCV with cross-validation.

Test accuracy:

84%

Confusion matrix:

| | Predicted No | Predicted Yes |
|---|---:|---:|
| Actual No | 1094 | 60 |
| Actual Yes | 175 | 183 |

Correct predictions:

1277 out of 1512

True Positive Rate:

51.1%

### Logistic Regression

Logistic Regression was trained using the same preprocessing pipeline and tuned using GridSearchCV.

Test accuracy:

83%

Confusion matrix:

| | Predicted No | Predicted Yes |
|---|---:|---:|
| Actual No | 1071 | 83 |
| Actual Yes | 174 | 184 |

Correct predictions:

1255 out of 1512

True Positive Rate:

51.4%

## Model Comparison

| Metric | Random Forest | Logistic Regression |
|---|---:|---:|
| Accuracy | 84% | 83% |
| Correct Predictions | 1277 | 1255 |
| True Positive Rate | 51.1% | 51.4% |

Random Forest achieved slightly higher overall accuracy, while Logistic Regression achieved a slightly higher true positive rate.

## Feature Importance

Random Forest feature importance analysis showed that Humidity3pm was the most important feature for rainfall prediction.

Other influential features included:

- Pressure3pm
- Pressure9am
- Sunshine
- WindGustSpeed
- Temp3pm
- MaxTemp
- MinTemp
- Temp9am
- Humidity9am

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Random Forest
- Logistic Regression
- GridSearchCV
- Machine Learning Pipelines

## Repository Structure

```text
rainfall-prediction-classifier/
│
├── FinalProject_AUSWeather.ipynb
└── README.md
