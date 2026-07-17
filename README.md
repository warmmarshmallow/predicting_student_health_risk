# 🩺 Kaggle Playground Series S6E7 – Health Condition Classification

A machine learning project for the **Kaggle Playground Series S6E7** competition focused on predicting an individual's **health condition** using demographic, lifestyle, and physiological features.

**Competition:** https://www.kaggle.com/competitions/playground-series-s6e7

---

## 📈 Results

| Metric | Score |
|---------|------:|
| Public Leaderboard | **0.81102** |

---

## 📖 Project Overview

The goal of this competition is to classify an individual's health condition from a mixture of numerical and categorical features.

This repository demonstrates a complete machine learning workflow, including:

- Exploratory Data Analysis (EDA)
- Data preprocessing
- Missing value handling
- Feature encoding
- Logistic Regression model training
- Kaggle submission generation

This project was completed as part of my journey learning applied machine learning and participating in Kaggle competitions.

---

## 📂 Repository Structure

```
.
├── visualization.ipynb      # Exploratory Data Analysis
├── test.ipynb               # Model training & submission
├── train.csv
├── test.csv
├── sample_submission.csv
├── submission.csv
└── README.md
```

---

## 🔍 Exploratory Data Analysis

The dataset was explored before model training to better understand feature distributions and relationships.

The EDA notebook includes:

### Target Distribution

- Class frequency visualization
- Class balance inspection

### Numerical Features

Boxplots and distribution plots for numerical variables such as:

- BMI
- Heart Rate
- Sleep Duration
- Water Intake
- Exercise Duration
- Daily Step Count

### Correlation Analysis

- Correlation heatmap
- Numerical feature relationships

### Categorical Features

Normalized bar charts for categorical variables including:

- Diet Type
- Physical Activity Level
- Sleep Quality
- Stress Level
- Smoking Status
- Alcohol Consumption
- Gender

### Feature Importance

Mutual Information scores were calculated to estimate the predictive strength of each feature.

---

## ⚙️ Data Preprocessing

The preprocessing pipeline performs several data-cleaning steps before training.

### Missing Values

**Numerical features**

- Filled using the median value.

**Categorical features**

- Filled using the most frequent category (mode).

### Feature Encoding

Categorical variables were converted into numerical features using **One-Hot Encoding**.

To ensure the training and testing datasets contain identical encoded columns, both datasets were combined before encoding and separated afterward.

---

## 🤖 Model

Current baseline model:

- Logistic Regression (Scikit-Learn)

Training workflow:

1. Load training and testing datasets
2. Handle missing values
3. Encode categorical variables
4. Split training data into training and validation sets
5. Train Logistic Regression
6. Evaluate validation performance
7. Generate predictions on the test set
8. Export predictions as `submission.csv`

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## 📊 Machine Learning Pipeline

```
Raw Data
      │
      ▼
Missing Value Imputation
      │
      ▼
One-Hot Encoding
      │
      ▼
Train / Validation Split
      │
      ▼
Logistic Regression
      │
      ▼
Prediction
      │
      ▼
submission.csv
```

---

## 🚀 Future Improvements

Future versions of this project may include:

- PyTorch Neural Networks
- CatBoost
- XGBoost
- LightGBM
- Hyperparameter tuning
- Feature engineering
- Cross-validation
- Ensemble learning

---

## 📚 What I Learned

This project helped reinforce my understanding of:

- Exploratory Data Analysis (EDA)
- Data visualization
- Missing value imputation
- One-Hot Encoding
- Feature preprocessing
- Mutual Information feature selection
- Logistic Regression
- Model evaluation
- Kaggle competition workflow
- Building complete machine learning pipelines

---

## 🏁 Conclusion

This project served as a practical introduction to solving a real-world tabular classification problem. Starting from raw data, I explored feature relationships, cleaned and encoded the dataset, trained a Logistic Regression baseline model, and generated Kaggle-ready predictions.

My first submission achieved a **Public Leaderboard score of 0.81102**, providing a strong baseline for future experimentation with more advanced machine learning models.
