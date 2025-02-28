# Genomics-Transformer-for-Diagnosing-Parkinson-s-Disease

📌 Project Overview

This project aims to reproduce and improve upon the findings of the research paper "Genomics Transformer for Diagnosing Parkinson’s Disease." Instead of using attention-based models, we experimented with various machine learning classifiers, including:

Logistic Regression (LR)

Random Forest (RF)

XGBoost

LightGBM

K-Nearest Neighbors (KNN)

CatBoost

The best-performing model, XGBoost, achieved an accuracy of 95.56%, outperforming other classifiers. Additionally, Explainable AI (XAI) tools like SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) were implemented to interpret model decisions and enhance transparency.

Dataset Information

Source: Publicly available PPMI dataset (Parkinson's Progression Markers Initiative).

Features: Clinical, biomarker, and genomic data.

Preprocessing Steps:

Missing values handled using KNN Imputation.

Categorical features encoded using Label Encoding.

Outlier detection & removal via Interquartile Range (IQR).

Dimensionality reduction using Principal Component Analysis (PCA).

⚠️ Note: The dataset is not included in this repository due to privacy constraints. If you need access, refer to the PPMI dataset link.

 Machine Learning Models Used

Model

Accuracy (%)

Logistic Regression

93.33

Random Forest

95.50

XGBoost

95.56 🏆

LightGBM

95.55

K-Nearest Neighbors (KNN)

67.40

CatBoost

94.81

📌 Best Model: XGBoost (Accuracy: 95.56%)


Explainable AI (XAI) Tools

To enhance model transparency, we integrated:

SHAP (SHapley Additive exPlanations) → Identifies feature importance for global and local predictions.

LIME (Local Interpretable Model-Agnostic Explanations) → Provides localized explanations for individual predictions.

📌 Key Findings from SHAP Analysis:

Mean Putamen was the most significant feature.

UPDRS3 Score and Mutation Status played a crucial role in predicting Parkinson’s Disease.


📝 Future Scope

🔹 Implement deep learning models like CNNs/RNNs for genomic sequence analysis.
🔹 Integrate ensemble techniques to improve prediction accuracy.
🔹 Apply advanced XAI techniques such as counterfactual explanations.
🔹 Validate models on larger, more diverse datasets for improved generalizability.
