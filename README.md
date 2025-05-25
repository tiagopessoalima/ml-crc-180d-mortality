# ML-Based 180-Day Mortality Prediction in Older Adults with Colorectal Cancer

This repository contains code and experiments from a study that developed a machine learning (ML) model to predict **180-day mortality in older adults with colorectal cancer (CRC)** using a combination of **Comprehensive Geriatric Assessment (CGA)**, **hematological markers**, and **tumor staging**.

## 🧠 Context

Older CRC patients present a complex prognosis shaped by frailty, systemic inflammation, and tumor burden. This project integrates clinical and lab data into ML models to improve early risk stratification and support clinical decision-making.

## 🎯 Objective

To develop and validate ML models that predict 180-day mortality post-admission in hospitalized older adults (≥60 years) with CRC.

## 📊 Dataset

- Cohort of 297 CRC patients treated at IMIP (2015–2022).
- Input features included CGA domains, hematological markers, and cancer staging.
- Preprocessing steps: normalization, imputation, class balancing.

## 🧪 Models Evaluated

- Decision Tree (DT)
- Gradient Boosting (GB)
- Logistic Regression (LR)
- Multi-Layer Perceptron (MLP)
- Naive Bayes (NB)
- Random Forest (RF)
- Support Vector Classifier (SVC)

Evaluation used **5-fold stratified cross-validation**, with **G-Mean** as the primary metric due to class imbalance.

## ✅ Best Model

The **Logistic Regression (LR)** model was selected based on its superior performance in:

- ROC AUC: **0.7855**
- Recall: **0.7096**
- G-Mean: **0.7241**

It demonstrated the best balance between sensitivity and clinical interpretability.

## 🔍 Key Predictors

Feature importance analysis from the LR model identified:

- Advanced tumor stage
- Low performance status (KPS)
- Malnutrition (MNA-SF)
- Elevated leukocyte count

## 📁 Repository Structure

├── abstract_11.ipynb # Notebook with data preparation, modeling, and evaluation
├── README.md # Project overview and documentation

