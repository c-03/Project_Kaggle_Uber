# Uber Ride Bookings Analysis

## Overview
This project utilises a Kaggle dataset — Uber Data Analytics Dashboard (ncr_ride_bookings.csv) to perform data analysis. This project includes data visualisation and predictive modelling in order to uncover what the booking status will be, given certain features. This would be useful for companies to consider how, for instance, Pickup and drop-off locations, Vehicle and customer time at arrival will affect a booking status to be completed or other statuses. 

## Dataset
- **File**: `ncr_ride_bookings.csv`
- **Source**: https://www.kaggle.com/datasets/yashdevladdha/uber-ride-analytics-dashboard/data?select=Dasboard.gif
- **Author**: Yash Dev Ladha

## Data Analysis Steps
- **Data Cleaning / Handling**
- **Data Visualisation**: Bar chart, Line Chart, Histogram, Correlation Matrix
= **Machine Learning**: Original data vs undersampling method with models (Decision Tree Classifier, Random Forest Classifier, XGBoost Classifier, Logistic Regression, Stochastic Gradient Descent Classifier [SGDC], Supper Vector Machine [SVM]) 

## Key Findings
- Undersampling has a higher accuracy compared to the origina imbalanced class training data. Yet, for f1 score, the differences is not very significant and it varies, depending on the selected model. 
- Ensemble Learning methods (Random Forest Classifier & XGBoost Classifier) have the highest accuracy, compared to other models. Yet, consider the time efficiency, Decision Tree Classifier might be the most computationally inexpensive choice with the most efficienct training time (6 times faster than Random Forest Classifier and 2 times faster than the XGBoost Classifier).
- SVM, SGDC and Logistic Regression on the other hand has a much lower accuracy and f1 score, indicating their ineffectiveness in this task.

## Project Author
This project was created for Kaggle Uber project by Alan Chan.
