# BetaBank Churn Prediction

## Project Overview
This project aims to develop a predictive model to identify customers likely to churn at Beta Bank. Since retaining existing customers is more cost-effective than acquiring new ones, Beta Bank wants to proactively reduce churn by focusing on at-risk clients. Using past customer behavior data, the model predicts the likelihood of churn and provides valuable insights to help Beta Bank implement targeted retention strategies.

## Objectives
- **Predict Customer Churn**: Analyze customer data to predict whether a client is at risk of leaving the bank.
- **Optimize Model Performance**: Aim for a high F1 score (minimum 0.59) to ensure accuracy in identifying at-risk customers, and evaluate model reliability using the AUC-ROC metric.

## Approach
- **Data Preprocessing**: Cleaned and prepared the dataset by handling missing values, encoding categorical features, and scaling numerical data for optimal model performance.
- **Model Selection**: Tested various machine learning algorithms, including Decision Tree, Logistic Regression, and Random Forest, and used grid search to optimize hyperparameters.
- **Evaluation Metrics**: Prioritized F1 score to balance precision and recall, with additional evaluation using AUC-ROC to assess model robustness.

## Tools and Libraries
- **Python Libraries**: `pandas`, `numpy`, `sklearn`, `matplotlib`, `seaborn`
- **Machine Learning Models**: Decision Tree, Logistic Regression, Random Forest
- **Techniques**: Grid Search for hyperparameter tuning, feature scaling, and categorical encoding

## Results
The project successfully implemented a churn prediction model that met the target F1 score, providing actionable insights into customer churn factors. This model enables Beta Bank to take proactive measures to retain valuable customers and improve overall business efficiency.

## Files in This Project
- **BetaBank.ipynb**: The Jupyter Notebook containing data exploration, preprocessing, model training, and evaluation.
- **Churn (1).csv**: Dataset containing customer behavior data used to train and test the model.
- **README.md**: Project description and documentation.
