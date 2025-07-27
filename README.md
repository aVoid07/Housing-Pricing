**Housing Price Prediction - End-to-End Machine Learning Project**
This repository contains a full-fledged ML project built on the California Housing Dataset. The notebook demonstrates the complete pipeline from data ingestion to model deployment readiness.

**Objective**
To predict median house values in Californian districts using various attributes such as population, median income, proximity to the ocean, etc.

**Workflow Overview**

1.  Data Acquisition & Loading
Dataset is fetched programmatically from an online repository.
Loaded using pandas into a DataFrame and explored for basic insights.

2.  Test-Train Split with Stable Hashing
Created a deterministic test set using a hashing technique for reproducibility.
Latitude and longitude are combined to generate a unique ID per row.

3.  Exploratory Data Analysis (EDA)
Used histograms, scatter plots, and correlation matrices to understand data distribution.
Geographic data visualized using scatter plots with alpha, c, and s attributes for better insights.

4.  Data Cleaning & Feature Engineering
Imputed missing values with median strategy.
Created new features such as:
rooms_per_household
bedrooms_per_room
population_per_household

5.  Pipeline Construction
Used Pipeline and ColumnTransformer to:
Handle numerical features (imputation + scaling).
One-hot encode categorical features (ocean_proximity).

6.  Model Training & Evaluation
Trained and evaluated:
Linear Regression
Decision Tree Regressor
Random Forest Regressor
Used cross_val_score and RMSE to evaluate performance.
Fine-tuned models using GridSearchCV.

**Tools & Libraries Used**
Python 3.x
NumPy, Pandas
Matplotlib, Seaborn
Scikit-learn

Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/housing-ml-project.git
cd housing-ml-project
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Launch the Notebook
bash
Copy
Edit
jupyter notebook "Housing - A Complete Project.ipynb"
📂 Repository Structure
cpp
Copy
Edit
.
├── Housing - A Complete Project.ipynb
├── README.md
└── requirements.txt (optional, can be generated)
📈 Sample Outputs
Feature importances plotted.

RMSE scores for each model compared.

Top hyperparameter combinations listed from GridSearchCV.

Author
Videh Jha

📄 License
This project is licensed under the MIT License.
