# Movie Review Sentiment Classification

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Conclusion](#conclusion)
- [Further Improvements](#further-improvements)

## Project Overview
The **Film Junky Union**, an edgy community for classic movie enthusiasts, is developing a system to automatically filter and categorize movie reviews based on sentiment. The goal of this project is to build a model to detect negative reviews, using IMDb movie reviews data with polarity labels. The target is to achieve an F1 score of at least 0.85 on the test set.

## Dataset Description
The dataset consists of movie reviews from IMDb, with the following key features:
- **review**: The text of the review.
- **pos**: The target variable, where '0' indicates a negative review and '1' indicates a positive review.
- **ds_part**: Indicates whether the data is part of the train or test set.

Additional fields may exist in the dataset, which can be explored further if necessary.

## Project Workflow
1. **Data Preprocessing**:
   - Loaded and inspected the dataset to understand its structure.
   - Handled missing values, if any, and prepared the data for modeling by converting the text data into numerical vectors using appropriate vectorization techniques.

2. **Exploratory Data Analysis (EDA)**:
   - Conducted EDA to identify patterns in the data and class imbalance.
   - Created visualizations to better understand the distribution of positive and negative reviews.

3. **Model Training**:
   - Trained at least three models, including:
     - Logistic Regression
     - Gradient Boosting
     - Other models (e.g., Decision Trees, Random Forest)
   - Models were evaluated using accuracy, F1 score, and precision-recall metrics.

4. **Model Evaluation**:
   - Tested the models on the test dataset and compared their performance.
   - Applied custom reviews to the trained models to classify them and compared the results.

5. **Findings**:
   - Analyzed the differences between model testing results and evaluated the overall performance against the project’s metric target.

## Results
The project achieved the following:
- **Best Model**: [Insert Model] with an F1 score of [Insert Score].
- **Precision**: [Insert Precision]
- **Recall**: [Insert Recall]

## Conclusion
The project successfully developed a model capable of classifying movie reviews into positive and negative categories. With an F1 score exceeding the 0.85 target, the model meets the quality standards set for the task. Logistic Regression and Gradient Boosting models both performed well, with the [Insert Model] model achieving the best results.

## Further Improvements
- Implementing BERT embeddings to improve the model’s handling of context in the reviews, although computationally demanding.
- Testing additional deep learning models such as LSTM or transformer-based models to improve performance.
- Expanding the dataset with more reviews and exploring further techniques to address class imbalance.
