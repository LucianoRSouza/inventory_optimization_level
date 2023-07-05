## ML Inventory Optimization Project

This repository contains the code and data for an inventory optimization project using machine learning techniques. The goal of the project is to optimize inventory levels based on historical sales data and other relevant factors.

### Project Overview

The project consists of the following steps:

1. Data Preparation: A dataset is created with the necessary data, including product information, locations, and historical sales data. Random data is generated for the demand rate and other variables.

2. Data Analysis: The dataset is analyzed to calculate total sales per year and generate insights into the sales trends.

3. Optimization Level Calculation: The optimization level is calculated based on the provided formula, considering variables such as demand rate, lead time, order cost, unit cost, and current inventory.

4. Monthly Aggregation: The data is aggregated monthly, grouping by year, month, product type, and location. Categorical features are encoded using LabelEncoder.

5. Model Training: The dataset is split into training and test sets. Several regression models (Linear Regression, Decision Tree Regressor, and Random Forest Regressor) are evaluated, and the best model is selected based on the root mean squared error (RMSE) on the test set.

6. Model Evaluation: The best model is evaluated on the test set, calculating metrics such as R-squared, mean squared error (MSE), mean absolute error (MAE), and RMSE. Sensitivity analysis is performed by perturbing a specific feature and observing the prediction difference.

### Results

The best model achieved an R-squared value of 0.9992 on the test set, indicating a high level of accuracy in predicting the optimization level. The root mean squared error (RMSE) was 0.257, indicating a small deviation from the actual values. The model also performed well on the training set, with an RMSE of 0.092 and an R-squared value of 0.9999.

### Usage

To use this code and replicate the results:

1. Clone the repository to your local machine.
2. Ensure that Python 3 and the required libraries (pandas, numpy, scikit-learn) are installed.
3. Run the `inventory_optimization.py` script to generate the dataset, perform data analysis, calculate the optimization level, and train the models.
4. Review the results and analysis in the console output.
5. Optionally, modify the code or dataset to fit your specific requirements.

### License

This project is licensed under the [MIT License](LICENSE).

Feel free to explore the code and data provided and adapt it to your own inventory optimization needs. If you have any questions or suggestions, please open an issue or reach out to the project maintainer.

