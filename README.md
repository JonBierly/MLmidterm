# MLmidterm

Taiwanese Bankruptcy Prediction - ML Midterm Project
Group Members: Aryan, Rowan, Jon, Nemo, and Jackson
Course: Foundations of Machine Learning
Date: 03/17/2025

Project Overview
This project aims to predict company bankruptcy using financial data from the Taiwan Economic Journal (1999-2009). We explored various machine learning models, including Logistic Regression, Random Forest, XGBoost, and SVM, to determine which best predicts bankruptcies.

Since bankruptcies are rare events (~3% of the dataset), we applied feature selection (PCA, Lasso), class balancing techniques, and threshold tuning to improve prediction accuracy.

Repository Structure:
Here’s where you can find everything:
- /notebooks/ → Jupyter Notebooks for EDA, feature selection, modeling, and evaluation
- /data/ → Processed dataset used for training and testing models
- README.md → Project documentation
- requirements.txt → List of dependencies to install

How to Run the Project
1. Install Dependencies
Ensure you have Python installed, then run:
pip install -r requirements.txt

2. Run the Jupyter Notebooks
Start Jupyter Notebook and open the notebooks directory:
jupyter notebook

Inside /notebooks/, run these notebooks in order:

EDA.ipynb → Exploratory Data Analysis & Feature Selection
Modeling.ipynb → Training & Evaluating Models
Threshold_Tuning.ipynb → Adjusting the decision threshold to improve recall

3. Running Models Directly (Without Jupyter)
python train_model.py


Key Findings:
Feature Selection: PCA was useful for dimensionality reduction, but Lasso kept original financial indicators, making models more interpretable.
Class Imbalance: Since only 3% of companies were bankrupt, models initially struggled to detect bankruptcies.
Best Model: XGBoost had the highest ROC-AUC score (0.918) but suffered from low recall.
Threshold Tuning: Lowering the decision threshold improved recall but increased false positives.


Slides: https://docs.google.com/presentation/d/1Rop5pMRIpiwnKTpdlsTJQkn8KqjzW18jkPbp2QuPUag/edit?usp=sharing



