# Alzheimer's Disease Risk Factor Analysis

This project analyzes data from over 2,000 patients to identify factors most strongly associated with Alzheimer's disease development. Using machine learning and statistical analysis, we demonstrate how data-driven approaches can enhance early detection strategies.

## Overview

- **Dataset:** alzheimers_disease_data.csv (2,149 patient records)
- **Source:** Kaggle - Alzheimer's Disease Dataset
- **Objective:** Identify significant predictors of Alzheimer's disease and develop accurate classification models


### Model Used and Performance Comparison
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 95.6% | 96.5% | 90.9% | 93.6% |
| Decision Tree | 92.3% | 89.5% | 88.9% | 89.2% |
| SVM | 90.7% | 90.7% | 82.4% | 86.3% |
| Logistic Regression | 83.3% | 79.1% | 71.9% | 75.3% |

- In the end, Random Forest was used

## Repository Contents

- analysis_notebook.ipynb - Complete Jupyter notebook with full analysis
- analysis_notebook.pdf - PDF export of the complete analysis
- alzheimers_disease_data.csv - Original dataset
- README.md - Project documentation

## Conclusion

Standardized clinical assessments are the most reliable predictors of Alzheimer's disease, significantly outperforming symptom-based indicators. **Cognitive and functional assessments remain the strongest predictors, significantly outperforming symptom-based indicators while also underscoring the importance of early screening and monitoring in aging populations.**