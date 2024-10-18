# Rusty Bargain Used Car Value Prediction

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Project Goals](#project-goals)
4. [Project Steps](#project-steps)
5. [Model Evaluation and Findings](#model-evaluation-and-findings)
6. [Conclusion](#conclusion)
7. [Future Work](#future-work)

---

## Project Overview
Rusty Bargain, a used car sales service, is developing an app that will allow users to quickly determine the market value of their cars. The goal of this project is to build a predictive model based on historical data that estimates car values. The prediction model needs to focus on three key aspects:
1. **Prediction quality**
2. **Prediction speed**
3. **Training time**

The dataset contains information about technical specifications, trim versions, and vehicle prices. This project evaluates different models and their hyperparameters to determine the best model for predicting car prices.

## Data Description
The dataset includes the following features:
- **DateCrawled**: Date when the profile was downloaded from the database.
- **VehicleType**: Vehicle body type.
- **RegistrationYear**: Vehicle registration year.
- **Gearbox**: Gearbox type.
- **Power**: Engine power (horsepower).
- **Model**: Vehicle model.
- **Mileage**: Mileage (in kilometers).
- **RegistrationMonth**: Vehicle registration month.
- **FuelType**: Type of fuel used by the vehicle.
- **Brand**: Vehicle brand.
- **NotRepaired**: Whether the vehicle has been repaired or not.
- **DateCreated**: Date when the profile was created.
- **NumberOfPictures**: Number of vehicle pictures.
- **PostalCode**: Postal code of the profile owner.
- **LastSeen**: Date of the last activity of the user.
- **Price** (target): Vehicle price (in Euros).

## Project Goals
1. **Develop predictive models** that estimate the price of used cars based on the dataset.
2. **Evaluate model performance** using the RMSE metric to measure prediction quality.
3. **Compare the speed and accuracy** of various models, focusing on tree-based algorithms like Random Forest and Gradient Boosting methods (LightGBM, CatBoost, XGBoost).
4. **Optimize hyperparameters** to improve model performance.

## Project Steps
1. **Data Preparation**:
   - Inspect the data and perform necessary preprocessing, such as handling missing values and converting data types.
   - Perform exploratory data analysis (EDA) to understand patterns in the data.

2. **Model Selection**:
   - Train multiple models, including:
     - Linear Regression (sanity check).
     - Decision Tree.
     - Random Forest.
     - LightGBM.
     - CatBoost and XGBoost (optional).
   - Tune hyperparameters for each model to optimize performance.
   - Compare model performance using the RMSE metric.

3. **Performance Evaluation**:
   - Analyze prediction quality and speed.
   - Measure training time for each model.
   - Choose the best model based on the evaluation criteria.

## Model Evaluation and Findings
- **Linear Regression**: Used as a baseline sanity check to ensure other models are working properly. The performance was suboptimal, as expected.
- **Random Forest**: Achieved good prediction quality with moderate training and prediction time.
- **LightGBM**: Performed well after hyperparameter tuning, providing a good balance between speed and prediction quality.
- **CatBoost/XGBoost**: Showed strong performance, particularly in terms of accuracy, but required longer training times.

## Conclusion
The best-performing model in terms of RMSE, speed, and training time was the **LightGBM model**. It provided accurate predictions while maintaining fast training and prediction times, making it an ideal choice for Rusty Bargain's app.

## Future Work
- **Further Hyperparameter Tuning**: Conduct more extensive hyperparameter tuning to improve model performance.
- **Advanced Feature Engineering**: Explore additional feature engineering techniques to improve the accuracy of the model.
- **Real-Time Prediction**: Implement the chosen model in a production environment to provide real-time predictions to app users.
