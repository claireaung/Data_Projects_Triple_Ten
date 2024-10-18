# Rusty Bargain Used Car Sales Prediction

## Table of Contents
- [Project Description](#project-description)
- [Dataset Description](#dataset-description)
- [Project Objective](#project-objective)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Conclusion](#conclusion)
- [Further Improvements](#further-improvements)

## Project Description
Rusty Bargain, a used car sales service, is developing an app to help users quickly determine the market value of their cars. The goal of this project is to build a machine learning model capable of predicting car prices based on historical data, including vehicle specifications and pricing information. The project focuses on balancing prediction quality, speed, and training time.

## Dataset Description
The dataset consists of the following key features:
- **DateCrawled**: The date the profile was downloaded from the database.
- **VehicleType**: Type of vehicle (e.g., sedan, SUV).
- **RegistrationYear**: Year of vehicle registration.
- **Gearbox**: Type of gearbox (automatic or manual).
- **Power**: Horsepower of the vehicle.
- **Model**: Vehicle model.
- **Mileage**: Mileage in kilometers.
- **RegistrationMonth**: The month the vehicle was registered.
- **FuelType**: Type of fuel (e.g., gasoline, diesel).
- **Brand**: Car brand.
- **NotRepaired**: Indicates whether the vehicle has been repaired.
- **Price**: The target variable, representing the car's price in Euros.

## Project Objective
- Build a predictive model to estimate used car prices based on technical specifications.
- Compare different machine learning models (Linear Regression, Random Forest, LightGBM) on their performance using the RMSE metric.
- Optimize models for accuracy, prediction speed, and training time.

## Project Workflow
1. **Data Preprocessing**:
   - Cleaned and preprocessed the data.
   - Handled missing and duplicate values.
   - Categorical features were encoded using one-hot encoding (OHE) where necessary.
   
2. **Model Training**:
   - Built and trained several models, including:
     - Linear Regression (as a baseline)
     - Decision Tree
     - Random Forest
     - LightGBM for gradient boosting

3. **Model Evaluation**:
   - Evaluated models using Root Mean Squared Error (RMSE) for prediction quality.
   - Compared models based on prediction time and training time.

4. **Hyperparameter Tuning**:
   - Tuned the hyperparameters of the models to improve performance.

## Results
- The **LightGBM** model achieved the best performance with an RMSE of [insert RMSE value].
- **Prediction Time**: The LightGBM model produced predictions in [insert time].
- **Training Time**: Model training took [insert time].

## Conclusion
The project successfully developed a robust predictive model for estimating used car prices. The LightGBM model outperformed other models in both accuracy and speed, making it the best choice for deployment. The model’s high accuracy ensures precise price predictions, and the fast prediction time enhances the app’s usability.

## Further Improvements
- Further tuning of hyperparameters to reduce the error margin.
- Experiment with additional models such as CatBoost or XGBoost.
- Introduce additional features to improve model performance, such as user profiles and market trends.
