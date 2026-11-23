# 🎗️ Breast Cancer Diagnosis Prediction

This repository contains a machine learning pipeline developed to predict breast cancer diagnosis (Malignant or Benign) based on computational cell nuclei features from the Wisconsin Diagnostic Breast Cancer (WDBC) dataset. This project explores the end-to-end data science lifecycle, focusing on robust data preprocessing, feature selection, and the comparative evaluation of multiple classification models.

## 🔬 Project Overview
Early and accurate diagnosis is critical in breast cancer treatment. This project utilizes quantitative features extracted from digitized images of fine needle aspirates (FNA) to build automated diagnostic models. The models aim to assist medical professionals by providing a secondary validation tool, analyzing 30 distinct cell nuclei characteristics such as radius, perimeter, and concavity.

**Key Challenges Addressed:**
*   **Data Preprocessing:** Handled non-linear feature distributions using the Yeo-Johnson transformation.
*   **Class Imbalance:** Applied Synthetic Minority Over-sampling Technique (SMOTE) exclusively on the training data to mitigate the inherent imbalance between Benign and Malignant cases without introducing data leakage.
*   **Multicollinearity:** Removed highly correlated features (correlation > 0.9) to improve model interpretability and reduce dimensionality.

## 🛠️ Methodology & Tech Stack
*   **Data Processing:** Python, Pandas, NumPy, Scikit-learn (StandardScaler, PowerTransformer)
*   **Class Balancing:** Imbalanced-learn (SMOTE)
*   **Visualization:** Matplotlib, Seaborn
*   **Machine Learning Models:**
    *   Support Vector Machine (SVM)
    *   Logistic Regression
    *   Random Forest
    *   XGBoost
    *   K-Nearest Neighbors (KNN)
    *   Gradient Boosting
    *   Decision Tree
    *   Naive Bayes

## 📊 Results & Model Selection
The models were evaluated using comprehensive metrics, including Accuracy, Precision, Recall, F1-Score, and ROC-AUC.
*   **Support Vector Machine (SVM)** achieved the highest overall performance with an accuracy of **98.25%**, perfect precision (**100%**), and an F1-Score of **97.56%**.
*   Correlation and feature importance analysis (via Random Forest) identified `radius_mean`, `concavity_worst`, and `concave_points_worst` as the most discriminative features for predicting malignancy.

## 📄 Full Documentation
For a detailed breakdown of the exploratory data analysis, preprocessing steps, and comprehensive evaluation metrics, please review the attached `Project_Report.pdf` and watch the presentation video here: [Project Presentation](https://youtu.be/nGWrbeZup8c).
