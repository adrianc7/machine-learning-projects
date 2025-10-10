# Near-Earth Objects (NASA) Hazard Classification Analysis

Predictive modeling project using NASA’s Near-Earth Object dataset to determine whether an asteroid is potentially hazardous.  
Developed multiple logistic regression models and dimensionality reduction methods to identify key orbital and physical factors correlated with hazard classification

## Overview
- Dataset: `nasa.csv` (asteroid data from NASA’s CNEOS / JPL)
- Goal: Predict asteroid hazard status and identify key predictors
- Methods: Logistic Regression, LASSO feature selection, PCA, VIF multicollinearity checks, cross-validation

## Data Preparation
- Cleaned and standardized all numerical features  
- Converted `Hazardous` to a binary target variable  
- Selected predictors using **LASSO (L1 regularization)** to remove redundant variables  
- Detected and removed highly correlated variables using **VIF** and correlation matrix thresholds (>0.9)

## Models and Performance
1. **Initial Logistic Regression:**  
   - Accuracy ≈ 0.83  
   - Low recall for hazardous asteroids (Class 1)

2. **PCA Logistic Regression:**  
   - Reduced to 5 principal components  
   - Accuracy ≈ 0.84  

3. **Reduced Logistic Model (after removing multicollinear features):**  
   - Accuracy ≈ 0.89  
   - Cross-validation mean ≈ 0.887  
   - Improved precision/recall balance across both classes

## Key Findings
- **Eccentricity:** negative correlation with hazard likelihood — more circular orbits increase risk.  
- **Minimum Orbit Intersection Distance (MOID):** positive correlation — closer orbital intersections indicate higher hazard risk.  
- Model’s mean predictive accuracy: **~89%**.

## Repository Contents
- `near-earth-objects-nasa.ipynb` — main notebook containing data preparation, feature selection, and model training  
- `near-earth-objects-nasa.pdf` — static exported notebook  
- `nasa.csv` — NASA Near-Earth Object dataset

