# Student Performance Analysis & Prediction using Machine Learning

**Author:** Khadija Anwer Hussain
**Course:** Data Science  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (Jupyter Notebook)

## Project Overview

This project studies which factors affect students' exam performance and tries to predict it with machine learning models.

- **Regression:** predict a student's *math score* (Linear Regression vs Random Forest)
- **Classification:** predict if a student will *Pass or Fail* (Logistic Regression vs Random Forest)

## Dataset

A practice dataset with the same structure as the Kaggle dataset *Students Performance in Exams* (1000 students). Columns: `gender`, `race/ethnicity`, `parental level of education`, `lunch`, `test preparation course`, `math score`, `reading score`, `writing score`.

## Steps in the Notebook

1. **Data Cleaning:** missing values, duplicates, text columns, score range and outliers
2. **Exploratory Data Analysis (EDA):** score distributions, test preparation, lunch type, parents' education, gender and correlation
3. **Regression models:** predicting the math score
4. **Classification models:** predicting Pass/Fail
5. **Conclusion** with findings and limitations

## Key Results

| Task | Best model | Result |
|---|---|---|
| Predict math score | Linear Regression | R² = 0.76, average error ≈ 6.3 points |
| Predict Pass/Fail | Logistic Regression | 71.0% accuracy (baseline 70.5%) |

- Students who completed the test preparation course and students with a standard lunch scored higher on average.
- Reading and writing scores are the strongest predictors of the math score.
- Background information alone is a weak predictor of Pass/Fail.

## Files

| File | Description |
|---|---|
| `Student_Performance_ML_Project.ipynb` | Main notebook with code, charts and explanations |
| `StudentsPerformance.csv` | Dataset |
| `students_cleaned.csv` | Dataset after cleaning, with the added `average_score` and `result` columns |

## How to Run

```
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
```

Open `Student_Performance_ML_Project.ipynb` and choose **Kernel → Restart & Run All**.
