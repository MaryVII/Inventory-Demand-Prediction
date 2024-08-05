# Inventory Demand Prediction

## 1. Business Understanding

### Problem Statement
Many companies face challenges in optimizing inventory holding costs and managing spare part stocks due to the unpredictable nature of spare part demand, which is influenced by downtime planning. Excessive inventory leads to waste, while poor planning results in shortages and unplanned downtime, affecting factory operations.

### Objective
To develop machine learning models that predict spare part demand for Rank A items based on time series data.

### Goal
Select the champion model that best predicts spare part demand.

## 2. Data Description & Attributions

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

## 3. Libraries Used

| Library       | Description                                                              |
|---------------|--------------------------------------------------------------------------|
| `pandas`      | Provides data structures and data analysis tools for Python.             |
| `numpy`       | Supports large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. |
| `matplotlib`  | A plotting library for creating static, animated, and interactive visualizations in Python. |
| `seaborn`     | Statistical data visualization library based on matplotlib.              |
| `hvplot`      | Provides a high-level plotting API for pandas and other data structures, built on HoloViews. |
| `scipy`       | A library used for scientific and technical computing, which includes modules for optimization, integration, interpolation, eigenvalue problems, and other tasks. |
| `gradio`      | A library for building machine learning web applications quickly and easily. |


