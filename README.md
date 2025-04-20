# Customer Satisfaction Analysis

This project analyzes customer satisfaction based on various factors such as product quality, delivery time, customer service, and website ease of use. The goal is to predict customer satisfaction (satisfied vs. not satisfied) based on available features using machine learning.

## Project Overview

The dataset used in this project contains information about customer purchases and their satisfaction ratings. The project includes the following steps:

1. **Data Preprocessing**: Clean the dataset by handling missing values and encoding categorical variables.
2. **Exploratory Data Analysis (EDA)**: Visualize the distribution of ratings, correlations, and the relationship between purchase amounts and satisfaction ratings.
3. **Model Training**: Train a Random Forest Classifier to predict customer satisfaction.
4. **Model Evaluation**: Evaluate the model using classification metrics like precision, recall, F1-score, and accuracy.
5. **Feature Importance**: Analyze the importance of different features in predicting customer satisfaction.

## Steps in the Project

### 1. Load the Dataset
The dataset is loaded from a CSV file and inspected for missing values and general information.

### 2. Data Preprocessing
- **Encoding categorical variables**: The 'LoyaltyProgramMember' and 'Gender' columns are converted into numeric values (`1` and `0`).
- **Handling missing values**: Missing values are checked and handled (if any).

### 3. Exploratory Data Analysis (EDA)
- **Distribution of Ratings**: The distribution of ratings across different aspects (Product Quality, Delivery Time, Customer Service, and Website Ease of Use) is visualized using histograms.
- **Correlation Heatmap**: A heatmap is generated to understand the correlation between various features in the dataset.
- **Purchase Amount vs. Satisfaction**: A scatterplot shows how the average satisfaction rating correlates with purchase amounts.

### 4. Feature Importance & Model Training
- A Random Forest Classifier is trained to predict whether a customer is satisfied or not, based on selected features such as `Age`, `Gender`, `PurchaseAmount`, `PurchaseFrequency`, `ReturnRate`, `DiscountUsage`, and `LoyaltyProgramMember`.
- A target variable (`Satisfaction`) is created based on the average rating across the product attributes.

### 5. Model Evaluation
- **Classification Report**: Shows metrics like precision, recall, and F1-score for model evaluation.
- **Confusion Matrix**: Displays the number of true positives, false positives, true negatives, and false negatives.
- **Accuracy Score**: The overall accuracy of the model.

### 6. Feature Importance Plot
- A bar plot is generated to show the importance of each feature in the prediction of customer satisfaction.

## Requirements

To run this project, you need to have the following Python libraries installed:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- imbalanced-learn

You can install these dependencies using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
