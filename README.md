# 🎓 Student Performance Analysis: Key Drivers of Academic Success

## 🌟 Project Overview

This project focuses on conducting an in-depth analysis of student academic performance using the provided dataset (`Expanded_data_with_more_features.csv`). The primary goal is to identify and quantify the impact of various socio-demographic and behavioral factors—such as **Parental Education**, **Weekly Study Hours**, and **Test Preparation**—on a student's final scores.

The analysis is performed using Python, specifically leveraging the power of **Pandas** for data manipulation and **Matplotlib/Seaborn** for insightful data visualization.

## 📊 Analysis Steps Performed (Methodology)

The project followed a standard data science pipeline:

### 1. Data Preprocessing & Cleaning
* **Missing Value Imputation:** Handled missing values in categorical columns like `EthnicGroup`, `ParentEduc`, and `WklyStudyHours` by filling them with 'Unknown' or using mode/median where appropriate.
* **Data Validation:** Ensured all score columns (`MathScore`, `ReadingScore`, `WritingScore`) were numeric.

### 2. Feature Engineering
New features were created to facilitate holistic performance analysis:
* `TotalScore`: The sum of scores across all three subjects.
* `AverageScore`: The student's overall mean score.
* `Result`: A categorical column determining the student's status as **Pass** or **Fail**, based on a minimum threshold (40 marks) in all three subjects.

### 3. Exploratory Data Analysis (EDA)
Visualizations (Bar Charts, Line Plots, Histograms) were used to explore correlations:

| Factor Analyzed | Key Finding |
| :--- | :--- |
| **Test Preparation** | Completing the TestPrep course resulted in significantly higher average scores (the strongest predictor). |
| **Parental Education** | A clear **positive correlation** was observed: student scores increase as parental education levels rise (e.g., from High School to Master's Degree). |
| **Weekly Study Hours** | Students studying **over 10 hours** per week achieved the highest average scores. |
| **Overall Performance** | Identified the overall Pass/Fail rate for the student cohort. |

## 🚀 How to Run the Project

### Prerequisites

You need Python installed on your system, along with the following libraries:

```bash
pandas
numpy
matplotlib
seaborn
