# Liver Disease Prediction – Applied Machine Learning Workflow

This repository explores the prediction of liver disease using clinical biomarkers, with a focus on building a reliable and interpretable machine learning workflow rather than optimizing purely for performance.

The project emphasizes disciplined preprocessing, feature scaling, class imbalance handling, and evaluation choices suited to a healthcare context. The objective is to demonstrate a clear, defensible approach to applied machine learning while highlighting common pitfalls in real-world modeling.

---

## Project Overview

The notebook implements an end-to-end classical machine learning workflow, including:

* Data loading and initial inspection
* Handling missing values and duplicate records
* Encoding categorical variables (e.g., Gender)
* Feature scaling using standardization
* Addressing class imbalance using SMOTE
* Train–test splitting for evaluation
* Training and comparison of multiple classification models
* Model evaluation using appropriate performance metrics

The project highlights how preprocessing decisions—such as scaling, encoding, and class balancing—can significantly influence model performance in healthcare datasets.

---

## Models Evaluated

The project trains and evaluates the following models:

* Logistic Regression
* Random Forest Classifier
* Support Vector Machine (SVM)

These models represent different modeling paradigms (linear, ensemble, and margin-based), enabling comparison under a consistent preprocessing framework.

---

## Evaluation Approach

Model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Given the medical context, particular attention is paid to recall to better assess the model’s ability to correctly identify liver disease cases and minimize false negatives.

---

## Handling Class Imbalance

The dataset exhibits class imbalance. To address this:

* SMOTE (Synthetic Minority Oversampling Technique) is applied
* The dataset is balanced prior to model training

*Note: In production settings, resampling should be applied only to the training data to avoid data leakage. This implementation prioritizes workflow simplicity for demonstration purposes.*

---

## Limitations and Scope

This project is intentionally scoped as an exploratory and portfolio-oriented exercise. Known limitations include:

* No cross-validation (single train–test split)
* Limited hyperparameter tuning
* Manual preprocessing instead of pipeline-based workflows
* No deployment or production inference system

These limitations reflect a focus on workflow clarity and conceptual understanding rather than production readiness.

---

## Dataset

The project uses the Indian Liver Patient Dataset, a commonly used dataset for educational and benchmarking purposes in healthcare-related machine learning tasks.

---

## Intended Audience and Use

This repository is intended to demonstrate:

* Practical understanding of applied machine learning workflows
* Awareness of preprocessing and evaluation challenges
* Ability to implement and compare baseline models

This project is shared for educational and portfolio purposes.
