# 🎓 Student Exam Score Prediction using Linear Regression

## 📌 Problem Statement
The objective of this project is to predict a student's exam score based on study hours, sleep hours, and attendance using Machine Learning.

---

## 📊 Dataset Description
This is a manually created dataset containing 20 rows.

### Input Features:
- Study_Hours (Number of hours studied per day)
- Sleep_Hours (Number of hours slept per day)
- Attendance (Percentage attendance)

### Target Variable:
- Exam_Score (Final exam score)

---

## 📈 Data Exploration
The following exploratory steps were performed:
- Displayed first and last 5 rows
- Checked dataset shape
- Checked data types
- Verified missing values
- Visualized data using:
  - Scatter Plot (Study Hours vs Exam Score)
  - Histogram (Distribution of Exam Scores)
  - Boxplot (Outlier detection)

---

## 🤖 Model Used
Linear Regression (from Scikit-learn)

### Steps:
1. Defined features (X) and target (y)
2. Split dataset into training and testing set (80-20 split)
3. Trained Linear Regression model
4. Evaluated using:
   - Mean Absolute Error (MAE)
   - R2 Score

---

## 📊 Results
MAE: 0.9390093654838516
R2 Score:0.9970604987119472

The R2 score indicates how well the model explains variation in exam scores.
A lower MAE shows better prediction accuracy.

---

## 🔬 Feature Experiment
Two experiments were conducted:

1. Removed Sleep_Hours feature and retrained model.
2. Added a new feature "Effort" (Study_Hours × Attendance) and retrained model.

Performance comparison showed that Study_Hours and Attendance have strong influence on exam scores.

---

## ⚠ Overfitting Check
The model was trained on the full dataset without train-test split.
This resulted in higher R2 score, demonstrating overfitting.

Using proper train-test split provides realistic performance evaluation.

---

## 🧠 Conclusion
Student performance is strongly influenced by study hours and attendance.
Linear Regression performs effectively for this dataset.
Feature engineering improved prediction performance.

---

## 🛠 Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
