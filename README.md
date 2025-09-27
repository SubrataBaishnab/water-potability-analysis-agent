Water Potability Prediction
This project analyzes a dataset containing various water quality parameters to predict whether water is potable (drinkable) or not. The analysis involves data loading, exploration, handling missing values, addressing class imbalance, and building several classification models to predict potability.

Dataset
The dataset used in this project is sourced from Kaggle: Water Quality and Potability. It includes the following features:

ph: pH of water (0 to 14)
Hardness: Hardness of water (mg/L)
Solids: Total Dissolved Solids (ppm)
Chloramines: Amount of Chloramines (ppm)
Sulfate: Amount of Sulfates (mg/L)
Conductivity: Electrical conductivity of water (μS/cm)
Organic_carbon: Amount of organic carbon in water (ppm)
Trihalomethanes: Amount of Trihalomethanes (μg/L)
Turbidity: Measure of the cloudiness or haziness of water (NTU)
Potability: Target variable - 0 (Not Potable) or 1 (Potable)
Project Structure
The project is structured as a Jupyter Notebook (or Google Colab notebook) that walks through the following steps:

Data Loading: Loading the water_potability.csv dataset.
Exploratory Data Analysis (EDA):
Checking for missing values.
Visualizing feature distributions using histograms.
Analyzing the correlation matrix between features.
Data Preprocessing:
Handling missing values by imputing with the median.
Addressing class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).
Data Preparation for Modeling:
Splitting the data into training and testing sets.
Scaling the features using StandardScaler.
Model Building and Evaluation:
Training and evaluating several classification models:
Logistic Regression
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Decision Tree
Random Forest
Evaluating models based on accuracy and classification reports.
Feature Importance Analysis: Analyzing the feature importance from the best-performing model (Random Forest).
Predictive Agent: Creating a function to predict the potability of new water samples using the trained Random Forest model.
Example Usage: Demonstrating how to use the predictive agent with sample data.
Requirements
To run this notebook, you will need the following Python libraries installed:

pandas
numpy
matplotlib
seaborn
scipy
sklearn
imblearn
kagglehub
