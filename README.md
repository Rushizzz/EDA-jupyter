# Project Overview
This project focuses on analyzing a dataset containing customer behavior data to predict a binary target variable indicating customer engagement. The analysis involves exploratory data analysis (EDA), feature importance identification, and the development of machine learning models.
## Dataset Description
The dataset contains the following columns:

| Column Name                | Description                                                  |
|----------------------------|--------------------------------------------------------------|
| Administrative             | Count of administrative pages viewed                         |
| Administrative_Duration    | Duration on administrative pages (in seconds)               |
| Informational              | Count of informational pages viewed                          |
| Informational_Duration     | Duration on informational pages (in seconds)                |
| ProductRelated             | Count of product-related pages viewed                        |
| ProductRelated_Duration    | Duration on product-related pages (in seconds)              |
| BounceRates                | Percentage of visitors who leave after viewing one page      |
| ExitRates                  | Percentage of visitors who exit the site                     |
| PageValues                 | Value of the page viewed (in monetary terms)                |
| SpecialDay                 | Indicator for special promotional days                       |
| Month                      | Month of the visit                                           |
| OperatingSystems           | Operating system used by the visitor                         |
| Browser                    | Browser used by the visitor                                  |
| Region                     | Geographic region of the visitor                             |
| TrafficType                | Type of traffic source                                       |
| VisitorType                | Type of visitor (Returning or New)                          |
| Weekend                    | Indicator if the visit occurred on a weekend                |
| Target                     | Binary target variable indicating customer engagement        |

## Objectives
### Exploratory Data Analysis (EDA):
Analyze the distribution of the target variable.
Identify patterns among visiting customers.
Examine correlations between key metrics such as exit rates and bounce rates.
Feature Importance Identification:
Determine which variables significantly impact the prediction of the target variable.
### Model Development:
Develop and compare various machine learning models to predict the target variable.
Select the best-performing model based on accuracy and other performance metrics.
### Requirements
To run this project, ensure you have the following Python libraries installed:
pandas
numpy
matplotlib
seaborn
scikit-learn
You can install these libraries using pip:
```pip install pandas numpy matplotlib seaborn scikit-learn```

### Usage Instructions
Load the Dataset: Use pandas to load the dataset from the CSV file.
Perform EDA: Utilize visualizations to explore data distributions and relationships.
Prepare Data for Modeling: Preprocess data by encoding categorical variables and splitting into training and testing sets.
Train Models: Implement various models such as Logistic Regression, Random Forest, and Decision Trees.
Evaluate Models: Compare model performance using accuracy scores and classification reports.

### Example Code Snippet
Here’s a brief example to get started with loading the data and performing basic EDA:
python
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv('Dataset-1.csv')

# Display first few rows
print(data.head())

# Plot distribution of Target variable
sns.countplot(x='Target', data=data)
plt.title('Distribution of Target Variable')
plt.show()
```
