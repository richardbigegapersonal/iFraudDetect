# iFraudDetect
End-to-End Fraud Detection System for Trappez Online Store Transactions

# 🕵️‍♂️ iFraudDetect – Trappez Online Store Fraud Detection System

**Project Goal**:  
A production-grade, end-to-end fraud detection pipeline for Trappez's online store. This system detects suspicious transactions, reduces monetary losses, and enhances the overall customer journey — built using modern MLOps best practices.

---

## 📌 Business Context
Trappez operates a high-volume e-commerce platform. Transactional fraud not only leads to revenue loss but also hurts customer trust and satisfaction. This project builds an intelligent detection system to identify fraudulent behavior based on transaction patterns, device fingerprints, user behavior, and other signals.

---

## 📂 Repository Structure

iFraudDetect/
├── data/ # Raw and processed datasets
│ ├── raw/
│ └── processed/
├── notebooks/ # Jupyter notebooks for EDA, modeling, and evaluation
├── src/ # Modular Python code
├── dashboards/ # Power BI reports
├── presentation/ # Executive slides for stakeholders
├── models/ # Trained and serialized model artifacts
├── .github/workflows/ # CI/CD and MLOps automation
├── requirements.txt # Python dependencies
└── README.md

yaml
Copy
Edit

---

## 🧪 Workflow Overview

### 🔹 Data Simulation
- Based on publicly available PaySim & Retail datasets
- Injected with synthetic fraud labels tailored for Trappez

### 🔹 EDA & Feature Engineering
- Exploratory visuals (heatmaps, pair plots, temporal aggregation)
- New features: transaction velocity, geo-device mismatch, anomaly scores

### 🔹 Modeling
- Models: Logistic Regression, XGBoost (main), optional deep learning
- Handled class imbalance with SMOTE and threshold tuning
- Explainability with SHAP

### 🔹 Deployment & MLOps
- Config-driven pipelines
- GitHub Actions for CI/CD
- Model tracking with MLflow (optional)
- Docker API (optional)

### 🔹 Business Reporting
- Executive dashboards in Power BI
- Monthly fraud trends, savings, recall precision KPIs

---

## 🚀 How to Run

### 1. Install Dependencies
```bash
pip install -r requirements.txt
