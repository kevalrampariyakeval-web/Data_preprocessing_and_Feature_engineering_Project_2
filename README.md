# 🏥 Healthcare Data Cleaning Project

## 📊 Handling Missing Values and Outlier Detection

### 📌 Project Overview

This project focuses on cleaning healthcare patient records by handling missing values and detecting/treating outliers. The dataset contains patient demographic and medical attributes with intentionally added missing values and synthetic outliers to simulate real-world healthcare data issues.

The goal is to prepare a clean and machine learning-ready dataset using multiple data preprocessing techniques.

---

## ❓ Problem Statement

As a Data Analyst in a healthcare company, the task is to process patient health records that contain:

* Missing values due to inconsistent reporting
* Outliers caused by measurement errors or unusual patient conditions

The final objective is to improve data quality for downstream machine learning tasks such as disease risk prediction.

---

## 🗂 Dataset Information

### 📋 Features Used

| Column Name    | Description                                   |
| -------------- | --------------------------------------------- |
| patient_id     | Unique patient ID                             |
| age            | Age of patient                                |
| gender         | Male / Female                                 |
| region         | Region of residence                           |
| bmi            | Body Mass Index                               |
| blood_pressure | Systolic Blood Pressure                       |
| cholesterol    | Cholesterol level                             |
| glucose        | Blood glucose level                           |
| disease_risk   | Target variable (0 = Low Risk, 1 = High Risk) |

---

## 🛠 Project Tasks

The project is divided into 3 parts:

---

# Part A: 🔍 Handling Missing Values

### ✅ Techniques Applied

### 1. Simple Imputer (Numerical)

Used mean imputation for:

* age
* bmi
* blood_pressure
* cholesterol
* glucose

### 2. Simple Imputer (Categorical)

Used most frequent value imputation for:

* gender
* region

### 3. Missing Indicator + Random Sample Imputation

* Created missing indicator columns
* Filled missing values using random sample values from existing data

### 4. KNN Imputer

Used K-Nearest Neighbors to estimate missing values based on nearest similar records.

### 5. MICE Algorithm

Used Multiple Imputation by Chained Equations for advanced multivariate missing value handling.

---

# Part B: 📈 Handling Outliers

### ✅ Methods Applied

### 1. Z-Score Method

Detected extreme values using standard deviation thresholds.

### 2. IQR Method

Used Interquartile Range to identify outliers.

### 3. Percentile Method

Detected extreme values using lower and upper percentile boundaries.

### 4. Winsorization Technique

Capped extreme values instead of removing them to preserve dataset size.

---

# Part C: 🧹 Final Clean Dataset

### 🎯 Final Output Includes

* No missing values
* Outliers treated properly
* Machine learning ready dataset
* Final cleaned CSV file exported

---

## 💻 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy
* Jupyter Notebook

---

## 📁 Files Included

| File Name                              | Description               |
| -------------------------------------- | ------------------------- |
| healthcare_patient_records.csv         | Raw dataset               |
| Healthcare_Data_Cleaning_Project.ipynb | Complete Jupyter Notebook |
| final_clean_healthcare_dataset.csv     | Final cleaned dataset     |
| README.md                              | Project documentation     |

---

## ▶️ How to Run

### Step 1

Download all project files.

### Step 2

Open Jupyter Notebook or Google Colab.

### Step 3

Open:

`Healthcare_Data_Cleaning_Project.ipynb`

### Step 4

Run all cells step by step.

---

## 🎯 Expected Outcome

By the end of this project:

* Missing values are handled using multiple methods
* Outliers are detected and treated
* Clean dataset is generated
* Data becomes suitable for machine learning models

---

## 📚 Learning Outcomes

This project helps in understanding:

* Data preprocessing
* Missing value imputation strategies
* Outlier detection techniques
* Data cleaning workflow
* Real-world healthcare analytics preparation

---

## 👨‍💻 Author

Project created for academic learning and practical implementation of Data Cleaning in Healthcare Analytics.

---

## 🚀 GitHub Submission Note

Before uploading to GitHub:

* Include screenshots of outputs
* Upload notebook, dataset, and README
* Keep folder structure clean
* Add clear project explanation

This improves project presentation and evaluation quality.
