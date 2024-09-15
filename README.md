# Predicting Bank Term Deposit Subscriptions Using Machine Learning

**Author:** Adel Hachani

## Executive Summary

This project analyzes a dataset from a Portuguese banking institution's direct marketing campaigns to predict whether clients will subscribe to a term deposit. By comparing the performance of four classification algorithms—K-Nearest Neighbors, Logistic Regression, Support Vector Machines, and Decision Trees—we aim to identify the most effective model and provide actionable insights to improve the bank's marketing strategies.

## Rationale

Effective prediction of client subscription to term deposits allows the bank to:

- **Optimize Marketing Campaigns:** Target high-potential clients to increase conversion rates and reduce costs.
- **Improve Customer Relationship Management:** Understand key factors influencing client decisions to tailor personalized marketing strategies.
- **Enhance Resource Allocation:** Allocate time, budget, and manpower more efficiently towards receptive client segments.

## Research Question

What factors influence a client's decision to subscribe to a term deposit, and which machine learning model best predicts client subscription based on these factors?

## Data Sources

The data used in this project comes from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing), specifically the "Bank Marketing Dataset" provided by a Portuguese banking institution. The dataset includes information collected from direct marketing campaigns conducted via phone calls.

- **Number of Instances:** 45,211
- **Number of Features:** 16 (including demographic information, contact details, and previous campaign outcomes)
- **Target Variable:** `y` (indicates whether the client subscribed to a term deposit)

## Methodology

The project involves the following steps:

1. **Data Preprocessing and Exploration:**
   - Handling missing values and zero values.
   - Encoding categorical variables.
   - Feature scaling and engineering.
   - Exploratory Data Analysis (EDA) to understand data distribution and relationships.

2. **Modeling:**
   - Implemented four classification algorithms:
     - K-Nearest Neighbors (KNN)
     - Logistic Regression
     - Support Vector Machines (SVM)
     - Decision Trees
   - Split data into training and test sets (80% training, 20% testing).
   - Trained models and made predictions.

3. **Evaluation:**
   - Evaluated models using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.
   - Performed cross-validation to ensure model robustness.
   - Analyzed model coefficients to understand feature importance.

## Results

- **Logistic Regression** emerged as the most effective model:
  - **Test Accuracy:** 89.10%
  - **Training Time:** Approximately 32 seconds
  - **Interpretability:** Provided insights into which features most influence client subscription.

- **Key Influential Features Identified:**
  - **Positive Influencers:**
    - Previous campaign success (`poutcome_success`)
    - Effective contact methods (`contact`)
    - Retired clients (`job_retired`)
    - Clients previously contacted (`previous_contacted`)
  - **Negative Influencers:**
    - Number of contacts during the campaign (`campaign`)
    - Existing housing loans (`housing`)
    - Existing personal loans (`loan`)
    - Zero account balance (`balance_zero`)

These insights can help the bank focus its marketing efforts on clients more likely to subscribe, optimize contact strategies, and tailor marketing messages to specific client segments.

## Next Steps

- **Hyperparameter Tuning:**
  - Further optimize model parameters to improve performance.

- **Explore Ensemble Methods:**
  - Consider models like Random Forests or Gradient Boosting Machines for potentially better accuracy.

- **Feature Engineering:**
  - Incorporate additional features or external data sources to enhance the model.

- **Deployment:**
  - Implement the model in a production environment and monitor its real-world performance.

- **Continuous Improvement:**
  - Regularly update the model with new data to maintain accuracy over time.

## Outline of Project

- [Data Preprocessing and Exploratory Analysis Notebook](https://github.com/ahachani/Comparing_Classifiers)
- [Modeling and Evaluation Notebook](https://github.com/ahachani/Comparing_Classifiers)
- [Insights and Recommendations Notebook](https://github.com/ahachani/Comparing_Classifiers)


## Contact and Further Information

For further information, please contact Adel Hachani at ahachani@yahoo.com.
