# 🎓 Student Performance Index Prediction using Linear Regression

Predicting students' academic **Performance Index** based on study habits, previous scores, sleep patterns, and extracurricular involvement using a Linear Regression model.

This project is part of my ongoing **Machine Learning learning series**, focused on mastering end-to-end regression workflows — from raw data to a fully evaluated model.

---

## 📌 Problem Statement

Academic performance depends on multiple lifestyle and study-related factors. This project builds a regression model to predict a student's **Performance Index** using features such as hours studied, previous scores, sleep hours, extracurricular activities, and practice question papers solved.

---

## 📊 Dataset

- **Source:** `Student_Performance.csv`
- **Rows:** 10,000
- **Features:**
  | Column | Description |
  |---|---|
  | Hours Studied | Number of hours the student studied |
  | Previous Scores | Score obtained in previous exams |
  | Extracurricular Activities | Yes/No |
  | Sleep Hours | Average sleep hours per day |
  | Sample Question Papers Practiced | Number of practice papers solved |
  | **Performance Index** | Target variable (continuous) |

---

## ⚙️ Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn
- **Model:** Linear Regression
- **Preprocessing:** MinMaxScaler, OneHotEncoder

---

## 🔍 Project Workflow

1. **Data Loading & Exploration** — Inspected structure, datatypes, and null values
2. **Feature-Target Split** — Separated independent features (`X`) and target (`y`)
3. **Outlier Detection** — Used boxplots to confirm no significant outliers were present
4. **Train-Test Split** — 80/20 split with `random_state=42`
5. **Feature Scaling** — Applied `MinMaxScaler` to normalize numerical columns
6. **Categorical Encoding** — Applied `OneHotEncoder` on `Extracurricular Activities`
7. **Correlation Analysis** — Identified `Previous Scores` and `Hours Studied` as the strongest predictors
8. **Model Training** — Trained a `LinearRegression` model on the processed data
9. **Model Evaluation** — Assessed performance using R², MAE, and RMSE on both train and test sets

---

## 📈 Results

| Metric | Train Set | Test Set |
|---|---|---|
| **R² Score** | 0.9887 | 0.9890 |
| **MAE** | 1.619 | 1.611 |
| **RMSE** | 2.042 | 2.021 |

The model generalizes well, with near-identical performance on train and test data — indicating no overfitting.

---

## 💡 Key Insights

- **Previous Scores** showed the strongest correlation (0.92) with Performance Index
- **Hours Studied** was the second strongest predictor (0.37)
- **Sleep Hours** and **Practice Papers** had minimal direct correlation with performance
- No outliers were detected, allowing normalization instead of robust scaling

---

## 📂 Repository Structure
├── Student_Performance.csv
├── model_train.ipynb
├── requirements.txt
└── README.md

---

## 👨‍💻 Author

**Udaya Kumar B Totta**

Computer Science Engineering Student  
Machine Learning | Data Science | Python Developer

---

⭐ If you found this project helpful, feel free to star the repository.