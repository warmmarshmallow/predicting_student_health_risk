# Kaggle Playground Series S6E7 - Health Condition Classification

This repository contains my solution for the Kaggle Playground Series S6E7 competition, where the goal is to predict an individual's health condition using demographic, lifestyle, and physiological features.

Competition Link: https://www.kaggle.com/competitions/playground-series-s6e7

## Results

| Model | Public Leaderboard |
|-------|-------------------:|
| Logistic Regression | **0.81102** |

## Project Structure

```
.
├── visualization.ipynb      # Exploratory Data Analysis
├── test.ipynb               # Model training and prediction
├── train.csv
├── test.csv
├── sample_submission.csv
├── submission.csv
└── README.md
```

## Exploratory Data Analysis

Before training the model, I explored the dataset to better understand the relationships between features and the target variable.

The analysis includes:

- Distribution of the target classes
- Correlation heatmap for numerical features
- Boxplots for numerical variables grouped by health condition
- Distribution of categorical variables
- Mutual Information feature importance

The visualizations are available in `visualization.ipynb`.

## Data Preprocessing

The preprocessing pipeline consists of:

- Filling missing numerical values using the median
- Filling missing categorical values using the mode
- One-hot encoding categorical variables
- Combining train and test datasets before encoding to ensure consistent feature columns
- Splitting the processed data into training and validation sets

## Model

The baseline model is implemented using Scikit-Learn's Logistic Regression.

Training pipeline:

1. Load and clean the data
2. Encode categorical features
3. Split into training and validation sets
4. Train Logistic Regression
5. Generate predictions for the test dataset
6. Export predictions as `submission.csv`

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

## Future Improvements

Possible improvements include:

- CatBoost
- XGBoost
- LightGBM
- PyTorch Neural Networks
- Hyperparameter optimization
- Feature engineering
- Cross-validation
- Ensemble methods

## Lessons Learned

Through this project I gained practical experience with:

- Exploratory Data Analysis (EDA)
- Missing value imputation
- One-hot encoding
- Feature preprocessing
- Logistic Regression
- Model evaluation
- Kaggle competition workflow
- Building end-to-end machine learning pipelines
