# House Prices and Disease Prediction Using Linear Regression

This repository contains the implementation of linear regression models for two datasets: one predicting house prices and the other analyzing disease progression. The goal of this project is to demonstrate how linear regression can be applied to real-world datasets for predictive analysis.

## Datasets

1. **House Prices Dataset (`house_prices.csv`)**
   - This dataset contains information on house prices with the following features:
     - **SqFt**: Area of the house in square feet
     - **Bedrooms**: Number of bedrooms
     - **Bathrooms**: Number of bathrooms
     - **Neighborhood**: The neighborhood where the house is located
     - **Price**: The price of the house

   The dataset consists of 128 samples and 5 features, which are used to predict house prices using linear regression.

2. **Diabetes Dataset (`diabetes.csv`)**
   - This dataset contains medical information about diabetic patients, with 442 samples and 11 features. The first 10 attributes are baseline variables (e.g., age, sex, body mass index, blood pressure, etc.), and the 11th attribute quantifies disease progression one year post-baseline. The goal is to predict disease progression based on the first 10 attributes using linear regression.

## Objectives

### Problem 1: House Price Prediction

1. **Data Preprocessing**:
   - Load the dataset into a pandas DataFrame.
   - Convert the categorical "Neighborhood" feature into a one-hot encoded format.
   - Split the dataset into training and test sets.
   
2. **Exploratory Data Analysis**:
   - Visualize relationships between the features using pair plots and heatmaps.
   - Investigate correlations between features and the target variable (price).
   
3. **Linear Regression Model**:
   - Use `sklearn`'s `LinearRegression` to train and evaluate the model on the dataset.
   - Evaluate the model performance using Root Mean Squared Error (RMSE).

### Problem 2: Diabetes Disease Progression Prediction

1. **Data Preprocessing**:
   - Load the diabetes dataset and preprocess it for linear regression.
   
2. **Gradient Descent Implementation**:
   - Implement linear regression from scratch using numpy, focusing on matrix operations.
   - Train the model using gradient descent and evaluate the performance using RMSE.

3. **Evaluation**:
   - Split the dataset into training and testing subsets.
   - Evaluate the model using RMSE and visualize the loss curves during training.
   - Perform multiple trials with different hyperparameters (e.g., learning rate, iterations) to analyze the impact on performance.

## Code Structure

- **`119010148_DDA3020_Homework1.ipynb`**: Jupyter Notebook implementing the linear regression model for both house price prediction and diabetes disease progression prediction.
- **`house_prices.csv`**: CSV file containing the house price dataset.
- **`diabetes.csv`**: CSV file containing the diabetes dataset.
- **`Task description.pdf`**: A PDF containing the task description and instructions for the homework assignment.

## Results

- **House Price Prediction**: The model’s performance is evaluated using RMSE on both the training and testing sets, providing insights into how well the model generalizes to unseen data.
- **Diabetes Disease Prediction**: The gradient descent implementation evaluates the effect of hyperparameters on RMSE, and the results are presented in training/testing RMSE as well as loss curves.

## Conclusion

This project showcases the use of linear regression to predict house prices and disease progression. By preprocessing the datasets, visualizing the relationships between features, and implementing gradient descent, the project provides a clear understanding of the model’s performance and the effect of hyperparameters.
