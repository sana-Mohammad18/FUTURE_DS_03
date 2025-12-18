# FUTURE_DS_03
Student Course Recommendation Prediction (Machine Learning Project)
📌 Project Overview

This project focuses on analyzing student satisfaction feedback data and building a machine learning model to predict the average satisfaction score for course-related questions based on rating distributions.

Unlike traditional student-level datasets, the given data is aggregated at the question level, where each record represents a feedback question along with the number of students who rated it from 1 to 5.
Based on this structure, a regression-based machine learning approach was chosen to accurately meet the task requirements.

🎯 Objectives

Understand student feedback patterns using aggregated survey data

Analyze how different rating weightages contribute to overall satisfaction

Build a predictive machine learning model to estimate average satisfaction scores

Evaluate model performance using appropriate regression metrics

Identify key factors influencing student satisfaction

📂 Dataset Description

The dataset contains aggregated student feedback with the following attributes:

Questions – Feedback question text

Weightage 1 to Weightage 5 (W1–W5) – Count of students giving ratings from 1 to 5

Total Feedback Given – Total responses for each question

Average / Percentage – Overall satisfaction score

Course Name / Basic Course – Course-related details

The dataset represents summary-level feedback, not individual student responses.

🛠️ Tools & Technologies Used

Python

Pandas & NumPy – data cleaning and manipulation

Matplotlib & Seaborn – data visualization

Scikit-learn – machine learning modeling

Jupyter Notebook / Google Colab

🔍 Methodology
1️⃣ Data Cleaning & Preparation

Handled file encoding issues (latin1)

Cleaned and standardized column names

Extracted numerical satisfaction scores from text-based fields

Selected rating weightages (W1–W5) as model features

2️⃣ Exploratory Data Analysis (EDA)

Analyzed distribution of rating weightages

Studied overall satisfaction patterns

Identified variations across feedback questions

3️⃣ Feature Engineering

Converted rating distributions into numerical feature vectors

Created a numeric target variable (Avg_Score) from average percentage values

4️⃣ Machine Learning Model

Built a Random Forest Regressor to predict average satisfaction scores

Chosen for its robustness, non-linearity handling, and interpretability

5️⃣ Model Evaluation

The model was evaluated using regression metrics, which are appropriate for continuous targets:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

6️⃣ Feature Importance Analysis

Extracted feature importance from the trained model

Identified which rating weightages contribute most to satisfaction scores

📊 Key Insights (Example)

Higher counts of 4 and 5 ratings significantly increase average satisfaction scores

Lower ratings (1 and 2) have a strong negative impact on overall satisfaction

Student satisfaction is more sensitive to higher-end ratings than lower ones

(Insights may vary based on actual model output.)

📁 Project Structure
├── data/
│   └── Student_Satisfaction_Survey.csv
├── notebooks/
│   └── task03_student_satisfaction_prediction.ipynb
└── README.md

🎉 Outcome

This project successfully demonstrates how aggregated survey data can be analyzed and used to build a predictive machine learning model.
The model provides valuable insights into student satisfaction trends and highlights the factors that most influence perceived course quality.

The project showcases practical skills in:

Data preprocessing

Exploratory data analysis

Machine learning regression

Model evaluation

Insight generation
