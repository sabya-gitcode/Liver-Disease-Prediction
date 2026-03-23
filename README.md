# Liver Disease Prediction – Applied Machine Learning Workflow

This repository presents an exploratory machine learning project focused on predicting the presence of liver disease using structured clinical data.

The project emphasizes a clear and disciplined machine learning workflow, with particular attention to data preprocessing, feature scaling, class imbalance handling, and evaluation choices suited to a healthcare context.

Rather than optimizing aggressively for maximum performance or complexity, the goal is to demonstrate a practical, well-reasoned approach to applied machine learning and highlight common pitfalls in real-world modeling.

---

## Project Overview

The notebook implements an end-to-end classical machine learning workflow, including:

- Data loading and initial inspection  
- Handling missing values and duplicate records  
- Encoding categorical variables (e.g., Gender)  
- Feature scaling using standardization  
- Addressing class imbalance using SMOTE  
- Train–test splitting for evaluation  
- Training and comparison of multiple classification models  
- Model evaluation using appropriate performance metrics  

All steps are implemented sequentially to reflect a transparent and interpretable workflow.

---

## Models Evaluated

The project trains and evaluates the following models:

- Logistic Regression  
- Random Forest Classifier  
- Support Vector Machine (SVM)  

These models represent different modeling approaches (linear, ensemble, and margin-based), allowing for comparison under a consistent preprocessing pipeline.

---

## Evaluation Approach

Model performance is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

Given the medical context, particular attention is paid to recall to better understand the model’s ability to correctly identify liver disease cases and reduce false negatives.

---

## Handling Class Imbalance

The dataset exhibits class imbalance. To address this:

- SMOTE (Synthetic Minority Oversampling Technique) is applied  
- Balancing is performed before model training  

This ensures that models are not biased toward the majority class.

---

## Limitations and Scope

This project is intentionally scoped as an exploratory and portfolio-oriented exercise. Known limitations include:

- No cross-validation (single train–test split)  
- Limited hyperparameter tuning  
- Manual preprocessing instead of pipeline-based workflows  
- No deployment or production inference system  

These limitations reflect a focus on clarity and learning rather than production readiness.

---

## Dataset

The project uses the Indian Liver Patient Dataset, a commonly used dataset for educational and benchmarking purposes in healthcare-related machine learning tasks.

---

## Intended Audience and Use

This repository is intended to demonstrate:

- Practical understanding of applied machine learning workflows  
- Awareness of preprocessing and evaluation challenges  
- Ability to implement and compare baseline models  

This project is shared for educational and portfolio purposes.
