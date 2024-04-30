data_analytics_project
==============================

# Data Analytics Course: FINAL PROJECT

## Defining the Problem

### Context
This dataset provides various information about patients, including age, gender, blood pressure, cholesterol levels, electrocardiographic (ECG) features, etc.

### Objective
The problem to be addressed with this dataset is to predict whether a person is less likely to have a heart attack (0) or if they are more likely to have a heart attack (1). Through data manipulation and exploration, we aim to find the type of data, identify nulls, outliers, the cardinality of the data, skewness, etc. With this, we seek a suitable database for the model to work optimally and correctly predict whether a person has a high or low chance of suffering a heart attack.

### Justification
Addressing heart attack prediction is crucial as it can save lives by enabling early interventions and lifestyle changes to reduce risk. Additionally, it helps minimize costs associated with treating heart attacks and improves medical care by personalizing care based on individual risk.

## Data Collection
- **Source:** This dataset was uploaded to Kaggle by the author Ali Rezaei. [Heart.csv](https://www.kaggle.com/datasets/arezaei81/heartcsv)
- **Description:** This is a public dataset provided in CSV format.

### Data Information:
- **Variables to Consider:**
  - age
  - sex
  - cp
  - trestbps
  - chol
  - fbs
  - restecg
  - thalach
  - exang
  - oldpeak
  - slope
  - ca
  - thal
- **Answer Variable:**
  - target (0 = less likely of heart attack, 1 = more likely of heart attack)

## Data Cleaning & Analysis
- Libraries used for data preparation, modeling, and analysis:
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Sklearn

## Data Preparation for Modeling
- Feature variables (X) and target variable (y) were defined.
- Train and test data were split using a 80/20 ratio.
- Data scaling was performed using StandardScaler to prevent variable preference due to scale differences.

## Modeling: Logistic Regression
- **Accuracy on Training Data:** 86%
- **Accuracy on Test Data:** 78%
- **Precision on Test Data:** 74%
- **Recall on Test Data:** 87%

## Modeling: Random Forest
- **Accuracy on Training Data:** 88%
- **Accuracy on Test Data:** 81%
- **Precision on Test Data:** 77%
- **Recall on Test Data:** 88%

## Modeling: Decision Trees
- **Accuracy on Training Data:** 84%
- **Accuracy on Test Data:** 78%
- **Precision on Test Data:** 73%
- **Recall on Test Data:** 77%

## Models Comparison
| Model | Accuracy | Precision | Recall |
|-------|----------|-----------|--------|
| LR    | 0.78     | 0.74      | 0.87   |
| RF    | 0.81     | 0.77      | 0.88   |
| DTree | 0.78     | 0.73      | 0.77   |

## Data Prediction
- After applying the Random Forest model to the data, only 118 out of 1024 values were predicted incorrectly.
- The percentage of wrongly predicted values is approximately 11%.

This indicates that the Random Forest model performed the best among the three models evaluated for this dataset.