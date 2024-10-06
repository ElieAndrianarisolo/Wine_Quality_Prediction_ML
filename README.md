# Wine Quality Prediction using Machine Learning

## Project Overview
This project focuses on predicting the quality of wine based on several chemical properties using machine learning techniques. The dataset contains multiple features that help in determining the wine quality, ranging from acidity to alcohol content. We employ data preprocessing methods such as outlier removal and then use a Random Forest Classifier to model and predict wine quality.

## Dataset
The dataset used for this project is the **Wine Quality Dataset** for red wine, which includes the following features:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality (target variable)

The target column, `quality`, consists of integer values representing the quality of the wine on a scale of 0 to 10.

## Project Workflow

1. **Data Loading**: 
   - The dataset is loaded using pandas (`winequality-red.csv`).
   
2. **Exploratory Data Analysis (EDA)**:
   - The dataset is analyzed using descriptive statistics and correlation matrices to understand the relationships among the features.
   - Missing values are checked, and there is a check for outliers using Z-scores.

3. **Outlier Removal**:
   - Z-scores are calculated, and data points with Z-scores greater than 3 are considered outliers and removed to improve model performance.

4. **Data Splitting**:
   - The cleaned data is split into features (X) and the target variable (Y).
   - The dataset is further split into training and test sets using an 80/20 ratio.

5. **Modeling**:
   - A Random Forest Classifier with 1000 estimators is used for classification.
   - The model is trained on the training dataset and then used to predict wine quality on the test dataset.

6. **Evaluation**:
   - The model's performance is evaluated using the accuracy score.


## Results
The Random Forest Classifier provides an accuracy score that helps evaluate how well the model predicts wine quality based on the features in the dataset.

