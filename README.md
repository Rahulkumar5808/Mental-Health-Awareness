# Mental-Health-Awareness
🧠 Mental Health in Tech - Data Analysis & Prediction

This project analyzes a real-world mental health survey dataset and builds a machine learning model to predict whether a person is likely to seek treatment for mental health issues, based on workplace conditions and personal demographics.

## 📊 Dataset Overview

- Source: Mental Health in Tech Survey (Open Source)
- Rows: 1259
- Columns: 25
- Topics include:
  - Demographics
  - Employment type and size
  - Remote work and benefits
  - Attitudes toward mental health
  - Treatment-seeking behavior

 ## 🧹 Data Cleaning Steps

- Dropped high-null and irrelevant columns (`comments`, `state`)
- Imputed missing values (`self_employed`, `work_interfere`)
- Cleaned and standardized `Gender`
- Encoded categorical variables for ML

 ## 🔍 Key Insights

- Smaller companies have higher treatment rates, possibly due to less formal support structures.
- Gender and remote work status are not strong predictors alone.
- Access to mental health **benefits** and **care options** are major factors.
- Fear of **consequences** at work discourages people from seeking help.

## 🧠 Machine Learning Model

**Model Used:** `RandomForestClassifier`  
**Target:** `treatment` (Yes/No)  
**Accuracy:** ~82%  

### 🔑 Top 5 Predictive Features:
- `work_interfere`
- `care_options`
- `mental_health_consequence`
- `benefits`
- `coworkers`

## 📈 Visualizations

Included various charts using `Seaborn` and `Matplotlib`, such as:
- Gender distribution
- Company size vs treatment
- Remote work vs treatment
- Correlation heatmap

---

## 🚀 Getting Started

### Requirements:
```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
