# Renewable Energy Prediction

## Project Overview

This project focuses on predicting whether renewable-energy availability will be **High or Low** using machine learning.

The project uses a renewable-energy dataset and applies data preprocessing, exploratory data analysis (EDA), data visualization, and a Decision Tree classification model.

## Objectives

- Clean and preprocess the renewable-energy dataset.
- Perform Exploratory Data Analysis (EDA).
- Visualize renewable-energy production patterns.
- Create High and Low energy-availability classes.
- Build a Decision Tree classification model.
- Evaluate the model using classification metrics.
- Identify important factors influencing renewable-energy availability.

## Dataset

The dataset contains **15,000 records and 13 variables**.

The main variables include:

- Renewable Energy Type
- Installed Capacity (MW)
- Energy Production (MWh)
- Energy Consumption (MWh)
- Energy Storage Capacity (MWh)
- Storage Efficiency (%)
- Grid Integration Level
- Initial Investment (USD)
- Funding Sources
- Financial Incentives (USD)
- GHG Emission Reduction (tCO2e)
- Air Pollution Reduction Index
- Jobs Created

## Data Preprocessing

The dataset was checked for:

- Missing values
- Duplicate records
- Data types
- Numerical values

The energy-availability target was created using the median energy production value.

Records with energy production greater than or equal to the median were classified as **High**, while the remaining records were classified as **Low**.

The resulting dataset contains:

- High: 7,500 records
- Low: 7,500 records

## Exploratory Data Analysis

The following visualizations were created:

- Energy production distribution
- Renewable-energy type comparison
- Boxplots
- Scatter plots
- Correlation heatmap
- High vs Low availability analysis

These visualizations were used to understand the relationships between renewable-energy production and the available features.

## Machine Learning Model

A **Decision Tree Classifier** was used to predict renewable-energy availability.

The model was configured using:

- Criterion: Entropy
- Maximum Depth: 5
- Random State: 42

## Model Performance

The Decision Tree model achieved the following results:

| Metric | Score |
|---|---:|
| Accuracy | 51.40% |
| Precision | 52.52% |
| Recall | 29.13% |
| F1-Score | 37.48% |

The results show that the current dataset provides limited predictive performance.

## Feature Importance

The most important features identified by the Decision Tree were:

1. Initial Investment
2. Installed Capacity
3. GHG Emission Reduction
4. Energy Storage Capacity
5. Storage Efficiency

## Conclusion

This project demonstrates how predictive analytics and data visualization can be used to study renewable-energy availability.

The Decision Tree model provides a basic High/Low classification approach. However, better prediction could be achieved by including additional environmental and time-based information such as temperature, solar radiation, wind speed, humidity, cloud cover, and historical energy generation.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
renewable-energy-prediction/
│
├── README.md
├── dataset/
├── code/
├── visualizations/
└── report/
