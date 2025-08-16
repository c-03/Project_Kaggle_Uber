# Uber Ride Bookings Analysis

## Overview
This project analyzes the **Uber Data Analytics Dashboard** dataset from Kaggle to uncover factors influencing ride booking status. Using data visualisation and predictive modeling, it explores how features like pickup/drop-off locations, vehicle type, and customer arrival time affect whether a booking is completed or has other statuses. The insights are valuable for optimizing ride-sharing operations.

## Dataset
- **File**: `ncr_ride_bookings.csv` (cleaned version: `ncr_ride_bookings_cleaned.csv`)
- **Source**: [Kaggle - Uber Ride Analytics Dashboard](https://www.kaggle.com/datasets/yashdevladdha/uber-ride-analytics-dashboard/data?select=Dasboard.gif)
- **Author**: Yash Dev Ladha
- **Description**: Contains ride booking data, including locations, vehicle types, timestamps, and booking statuses.

## Data Analysis Steps
1. **Data Cleaning**:
   - Handled missing values, outliers, and inconsistencies in `ncr_ride_bookings.csv`.
   - Generated `ncr_ride_bookings_cleaned.csv` for analysis.
2. **Data Visualisation**:
   - **Python (Jupyter Notebook)**:
     - **Bar Chart**: Visualizes the distribution of booking statuses (e.g., completed, canceled).
     - **Line Chart**: Shows trends in ride bookings over time.
     - **Histogram**: Displays distributions of ride distances or times.
     - **Correlation Matrix**: Highlights relationships between numerical features (e.g., distance, time).
   - **Tableau**:
     - **Dashboard**: Interactive visualisations in `Uber-Analyis_Dashboard.twbx`, including user behavioural observation and Uber's KPIs.
3. **Predictive Modeling**:
   - Compared original imbalanced data vs. undersampling.
   - Models: Decision Tree, Random Forest, XGBoost, Logistic Regression, Stochastic Gradient Descent (SGDC), Support Vector Machine (SVM).

## Key Findings
- **Undersampling vs. Original Data**:
  - Undersampling improves accuracy but has minimal impact on F1 score, varying by model.
- **Model Performance**:
  - Ensemble methods (Random Forest, XGBoost) achieve the highest accuracy.
  - Decision Tree is the most computationally efficient (6x faster than Random Forest, 2x faster than XGBoost).
  - Logistic Regression, SGDC, and SVM show lower accuracy and F1 scores, indicating limited effectiveness for this task.
- **Applications**: Insights can help optimize ride allocation, predict cancellations, and improve operational efficiency.

## Visualisations
- **Python Outputs** (in `Uber-Analysis.ipynb`):
  - `booking_status_distribution_with_pct.png`: Bar chart showing the percentage distribution of booking statuses.
  - `correlation_matrix.png`: Heatmap of feature correlations, identifying key relationships.
- **Tableau Dashboard** (in `Uber-Analyis_Dashboard.twbx`):
  - Interactive visualisations of user behavioural pattern for drivers and Uber.
  - Download and open in Tableau Desktop or Tableau Public to explore.

## Files
- `ncr_ride_bookings.csv`: Raw dataset.
- `ncr_ride_bookings_cleaned.csv`: Cleaned dataset for analysis.
- `Uber-Analysis.ipynb`: Jupyter Notebook with data cleaning, visualisations, and predictive modeling.
- `Uber-Analyis_Dashboard.twbx`: Tableau workbook with interactive dashboards.
- `requirements.txt`: Python dependencies.