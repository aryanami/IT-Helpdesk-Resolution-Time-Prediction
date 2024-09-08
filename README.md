# IT-Helpdesk-Resolution-Time-Prediction

##Overview 
This project aims to develop a predictive model for IT helpdesk ticket management, leveraging historical data to classify tickets and predict their resolution time. The goal is to enhance operational efficiency, optimize resource allocation, and set realistic expectations for issue resolution times.

##Problem Statement  
Modern organizations rely on efficient ticket management systems to maintain operational efficiency and customer satisfaction. This project focuses on creating a statistical model to predict the time required to resolve IT helpdesk tickets, aiding organizations in improving ticket management processes.

##Dataset 
The dataset used for this project is sourced from Kaggle, containing IT Service Management data with details about incident tickets. Key features include ticket category, priority, severity, and requestor details.

##Challenges 
Missing Values: Rows with missing data were removed to maintain accuracy.
Inconsistent Values: Inconsistencies like non-numeric entries were standardized.
Noisy Data: Outliers were detected and removed using Z-score analysis.
Complex Data Relationships: Multiple factors influencing resolution time were managed through careful preprocessing.

##Data Preprocessing 
Data Cleaning: Removed rows with null values and outliers.
Standardization: Scaled numeric values using StandardScaler to ensure uniform feature influence.
Data Type Conversion: Converted categorical data to numeric values for model compatibility.
Encoding: Used label encoding and one-hot encoding for categorical features.
Feature Selection: Employed correlation matrix and feature importance plots to select key features.

##Models Used  
1. Multi-Linear Regression (MLR)
2. Support Vector Regression (SVR)
3. Random Forest Regression (RF)
The Random Forest Regression model outperformed others, with an accuracy of 77%, making it the chosen model for further analysis.

##Why Random Forest?  
Handles non-linear relationships well.
Robust against overfitting due to ensemble learning.
Provides feature importance analysis, aiding in model interpretability and optimization.
Exhibits high generalizability to unseen data.

##Results 
The model accurately predicts ticket resolution times, as validated against a test dataset. The predictions support better management of ticket assignment and contribute to increased customer satisfaction by setting realistic expectations and optimizing resource allocation.
