# Social Network Ads Dataset Analysis and Perceptron Classification

This project analyzes the Social Network Ads dataset using data visualization techniques and applies a Perceptron classifier to predict whether a user purchased a product based on their age and estimated salary.

## Project Overview

The project involves the following steps:

### Data Exploration and Visualization

1. Loaded the dataset (`Social_Network_Ads.csv`) using Pandas.
2. Explored the dataset's shape and first few rows to understand its structure.
3. Visualized relationships between features and the target variable (`Purchased`) using Seaborn:
   - Bar plots showing the relationship between `Purchased` and `Age`, `EstimatedSalary` with respect to `Gender`.
   - Scatter plot of `Age` vs `EstimatedSalary` colored by `Purchased`.

### Data Preprocessing

1. Balanced the dataset by downsampling the majority class (`Purchased=0`) to match the minority class (`Purchased=1`).
2. Standardized the features (`Age` and `EstimatedSalary`) using `StandardScaler` from scikit-learn.

### Model Training and Visualization

1. Trained a Perceptron classifier using the standardized features (`Age` and `EstimatedSalary`) and the target variable (`Purchased`).
2. Plotted the decision boundaries using `plot_decision_regions` from `mlxtend.plotting` to visualize how the Perceptron classifies the data based on age and estimated salary.
