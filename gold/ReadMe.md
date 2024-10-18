# Gold Recovery Prediction Project

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Conclusion](#conclusion)
- [Further Improvements](#further-improvements)

## Project Overview
This project aims to develop a predictive model to forecast the recovery rates of gold at different stages of processing. The raw data is provided in three files and consists of parameters collected during the extraction and purification of gold, silver, and lead. The goal is to prepare the data, analyze it, and develop a model that can predict the efficiency of recovery during different stages of the production process.

## Dataset Description
The dataset is provided in three CSV files:
- **gold_recovery_train.csv**: Training data.
- **gold_recovery_test.csv**: Testing data without target features.
- **gold_recovery_full.csv**: Full dataset containing both training and test data with all features.

The data contains measurements indexed by acquisition date and time. Some features are only available in the training set, and the test set lacks the target features necessary for prediction. The primary target is to predict the recovery rate (rougher.output.recovery).

## Project Workflow
### 1. Data Preparation
- **1.1.** Opened the files and examined the data structure.
- **1.2.** Verified the calculation of the recovery rate for the rougher.output.recovery feature using the training set. The Mean Absolute Error (MAE) between calculated values and the feature values was computed.
- **1.3.** Analyzed the features that were unavailable in the test set and their types.
- **1.4.** Performed data preprocessing, including handling missing values, checking for outliers, and removing irrelevant features.

### 2. Data Analysis
- **2.1.** Analyzed the change in metal concentrations (Au, Ag, Pb) across different purification stages.
- **2.2.** Compared feed particle size distributions between the training and test sets to identify discrepancies that could lead to model evaluation errors.
- **2.3.** Investigated the total concentration of all substances at various stages (raw feed, rougher concentrate, final concentrate). Detected and eliminated abnormal values in the total distribution.

### 3. Model Building and Evaluation
- **3.1.** Developed a function to calculate the final Symmetric Mean Absolute Percentage Error (sMAPE) value.
- **3.2.** Trained multiple models using cross-validation, including Random Forest and Gradient Boosting methods. The models were evaluated based on the sMAPE metric, and the best model was selected for testing on the test set.

## Results
- The final model achieved an sMAPE value of [Insert sMAPE Value] on the test dataset.
- The predictive accuracy of the model was validated through cross-validation, with the best-performing model being [Insert Model Name].

## Conclusion
The project successfully developed a predictive model to forecast gold recovery rates, achieving the desired accuracy based on the sMAPE metric. The analysis of metal concentrations and purification stages provided insights into the data, which helped in building a reliable model.

## Further Improvements
- Additional feature engineering to incorporate more complex relationships between variables.
- Exploration of deep learning models such as neural networks to further improve predictive accuracy.
- Refinement of the data preprocessing pipeline, especially around missing values and outlier handling.
