
# 🩺 Diabetes Data Mini-Project

This repository contains my final capstone project from my 3 day mini-project exploring the [Pima Indian Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database). I used this project to practice data cleaning, feature engineering, and basic visual analytics using **pandas**, **matplotlib**, and **seaborn** in Google Colab.

---

## 📌 Project Summary

Over the last day i finalised my pandas lessons whic can be viewed in this repo [pandas-diabetes-analysis](github.com/thisismcgovern/pandas-diabetes-analysis), I analyzed how patient data—such as glucose levels, BMI, and age—relate to diabetes outcomes. I approached this in stages: first inspecting and cleaning the data, then engineering new features, and finally performing analysis and visualizations to generate insights. My goal was to extract meaningful patterns and simulate advising a medical clinic based on real-world patient data.

---

## 🚀 What I Did

### 📦 Importing and Loading

* Imported all necessary libraries (`pandas`, `seaborn`, `matplotlib`)
* Loaded the dataset using `files.upload()` in Google Colab

### 🔍 Data Inspection

* Used `.head()`, `.tail()`, `.describe()` and `.info()` to understand the structure
* Identified columns with placeholder zeroes (like Glucose, Insulin) and cleaned them by replacing zeros with `NaN`
* Imputed missing values using median values for numeric columns

### 🔧 Feature Engineering

* Created new columns:

  * `BMI_Class`: Categorized BMI into Underweight, Normal, Overweight, and Obese
  * `Glucose_Level`: Labeled glucose values as Normal, Pre-diabetic, or Diabetic
  * `Age_Group`: Grouped patients into <30, 30–40, 40–50, and 50+ years

### 📊 Analysis

* Grouped and analyzed average values by:

  * Age groups
  * BMI class
  * Glucose levels
* Created pivot tables to compare glucose levels by age and diabetes outcome
* Generated bar plots and boxplots to visualize BMI and glucose distributions by outcome

### 🧠 Key Insights

* Diabetic patients (Outcome = 1) consistently showed higher BMI and Glucose
* The 50+ age group with diabetes had the highest average glucose
* Some patients with low or normal BMI were still diabetic—BMI isn’t a sole predictor

---

## ✅ Clinic Recommendations (Based on Findings)

* **Screen all patients aged 50+ regularly**, especially those with high BMI
* **Don’t rely solely on BMI**—use glucose and insulin tests even for patients with normal weight
* **Introduce early education** for patients aged 30–50 to prevent prediabetic progression

---

## 📁 Files

* `diabetes_day3_analysis.ipynb`: Main Colab notebook for Day 3 (data cleaning, feature engineering, insights)
* `diabetes.csv`: Dataset used (uploaded manually in Colab)

---

## 🧪 Tools Used

* Python 3, Pandas
* Seaborn & Matplotlib for visualization
* Google Colab

---

> *"This project take my first steps data engineering and ml plus aiding my understanding of how to approach real-world health datasets, clean them properly, engineer features, and draw conclusions that matter."* – McGovern

---

Let me know if you'd like this converted directly into a `.md` file or if you'd like it customized even further for GitHub.
