# Housing Price Prediction – End-to-End Machine Learning Project

This repository contains a comprehensive machine learning project built using the California Housing dataset. It demonstrates the complete ML lifecycle — from data acquisition and exploration to model training, evaluation, and deployment readiness.

---

## Project Objective

To develop a predictive model that estimates median housing prices in California districts based on features such as population, median income, and proximity to the ocean. The project emphasizes clean preprocessing, feature engineering, model interpretability, and pipeline automation.

---

## Dataset Overview

* **Source**: California Housing dataset (via Scikit-learn)
* **Features**:

* Numerical: median income, housing age, total rooms, bedrooms, population, households, etc.
* Categorical: `ocean\_proximity`
* **Target**: `median\_house\_value`

---

## Workflow Overview

### 1. Data Acquisition

* Dataset programmatically downloaded and loaded into a pandas DataFrame.
* Reproducible test-train split implemented using hashing on latitude-longitude combinations.

### 2. Exploratory Data Analysis (EDA)

* Visualizations used to understand feature distributions and detect correlations.
* Scatter plots, histograms, and heatmaps used to uncover geographic and socioeconomic patterns.

### 3. Data Cleaning and Feature Engineering

* Missing values handled using median imputation.
* New features created for better model representation:

* `rooms\_per\_household`
* `bedrooms\_per\_room`
* `population\_per\_household`

### 4. Pipeline Construction

* Employed `Pipeline` and `ColumnTransformer` from Scikit-learn to automate preprocessing:

* Numerical features: imputation and scaling
* Categorical features: one-hot encoding

### 5. Model Training and Evaluation

* Models Trained:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Evaluation Metrics:

* Cross-validated RMSE (Root Mean Squared Error)
* Hyperparameter tuning performed using `GridSearchCV`

### 6. Final Output and Interpretability

* Feature importance plotted for Random Forest.
* RMSE comparison across models.
* Final pipeline is exportable for deployment.

---

## Tools and Technologies

* **Languages**: Python 3.x
* **Libraries**: pandas, NumPy, matplotlib, seaborn, scikit-learn
* **Concepts**: regression, data preprocessing, feature engineering, model tuning, pipeline design

---

## Repository Structure

```
.
├── Housing - A Complete Project.ipynb
├── README.md
```

---

## Key Highlights

* Full ML pipeline from ingestion to model selection and evaluation
* Reproducible data splitting and clean feature engineering
* Automation using Scikit-learn Pipelines and ColumnTransformers
* Interpretability and performance analysis using visual and statistical tools

---
