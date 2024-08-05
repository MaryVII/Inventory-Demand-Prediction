# Inventory Demand Prediction for Manufacturing Company A

## 1. Business Understanding

### Problem Statement
Many companies face challenges in optimizing inventory holding costs and managing spare part stocks due to the unpredictable nature of spare part demand, which is influenced by downtime planning. Excessive inventory leads to waste, while poor planning results in shortages and unplanned downtime, affecting factory operations.

### Objective
To develop machine learning models that predict spare part demand for Rank A items based on time series data.

### Goal
Select the champion model that best predicts spare part demand.

## 2. Analytic Approach

### 1. Data Collection and Data Wrangling
- **Data Sources**: Gather relevant time series data from Company A, including historical demand data, downtime records, inventory levels, and other pertinent factors.
- **Data Wrangling**: Address missing values, outliers, and inconsistencies to ensure data is in an appropriate format for analysis.

### 2. Exploratory Data Analysis (EDA)
- **Trend Analysis**: Explore historical demand trends, seasonal patterns, and anomalies.
- **Visualization**: Create plots to visualize demand patterns, seasonality, and feature relationships.
- **Correlation Analysis**: Evaluate how various features correlate with demand to guide feature selection.

### 3. Model Selection and Development
- **Model Types**: Evaluate a range of machine learning and time series models, including:
  - Linear Regression
  - Polynomial Regression
  - Decision Tree
  - Random Forest
  - XGBoost
- **Model Training**: Split data into training and validation sets. Train and fine-tune models using the training data.
- **Cross-Validation**: Use cross-validation to assess model performance and prevent overfitting.

### 4. Model Evaluation
- **Metrics**: Use evaluation metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared to measure model accuracy.
- **Comparison**: Compare model performance using these metrics to identify the best-performing model.

### 5. Model Selection
- **Champion Model**: Choose the model with the best performance based on evaluation metrics.
- **Interpretation**: Analyze results to understand predictions and validate with domain knowledge.

### 6. Implementation and Monitoring
- **Deployment**: Implement the champion model for real-time forecasting or periodic updates.
- **Monitoring**: Continuously monitor model performance and adjust based on feedback and new data.

### 7. Reporting and Documentation
- **Results**: Document findings, including model selection, performance metrics, and recommendations.
- **Presentation**: Prepare detailed reports or presentations to communicate results and insights to stakeholders.

## 3. Data Requirements

| Parameter           | Description                                           | Type of Attribute |
|---------------------|-------------------------------------------------------|-------------------|
| Material            | Spare part unique ID number                          | Categorical       |
| Material Description | Spare part detail description registered in the system | Categorical       |
| Net Price           | Price of item per purchase per unit                  | Numerical         |
| Currency            | Currency of purchase transaction                     | Categorical       |
| Entry Unit          | Stock keeping unit of item                           | Categorical       |
| GI Date             | Date of spare part usage transaction                 | Object            |
| Month               | The month of spare part usage transaction            | Categorical       |
| Year                | Year of spare part usage transaction                 | Categorical       |
| Storage Location    | Central warehouse location                           | Categorical       |
| GI/GR Qty           | Spare part usage quantity                            | Numerical         |
| GI/GR Pr            | Spare part usage price                               | Numerical         |
| Cost Centre         | Department charged for the usage transaction         | Categorical       |
| Receiving Plant     | Factory charged for the usage transaction            | Categorical       |
| Material Document   | Transaction unique ID number                         | Categorical       |

## Libraries Used

| Library       | Description                                                              |
|---------------|--------------------------------------------------------------------------|
| `pandas`      | Provides data structures and data analysis tools for Python.             |
| `numpy`       | Supports large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. |
| `matplotlib`  | A plotting library for creating static, animated, and interactive visualizations in Python. |
| `seaborn`     | Statistical data visualization library based on matplotlib.              |
| `hvplot`      | Provides a high-level plotting API for pandas and other data structures, built on HoloViews. |
| `scipy`       | A library used for scientific and technical computing, which includes modules for optimization, integration, interpolation, eigenvalue problems, and other tasks. |
| `gradio`      | A library for building machine learning web applications quickly and easily. |


