# 🍄 Mushroom Classification

This repository contains a machine learning project for classifying mushrooms as **poisonous (p)** or **edible (e)** using physical and categorical features.

## 📌 Project Overview
- **Dataset**: Mushroom features (`train.csv`, `test.csv`)  
- **Goal**: Predict whether a mushroom is poisonous or edible  
- **Model**: `HistGradientBoostingClassifier`  
- **Output**: `sample_submission.csv` with predicted labels (`p` or `e`)  

## ⚙️ Steps in the Pipeline
### 🔹 Data Preprocessing
- Encode categorical features (yes/no, season, multi-categorical attributes)  
- Handle missing values with median imputation  
- Frequency encoding for complex categorical features  

### 🔹 Feature Engineering
- Binary & multi-category transformations  
- Season encoded with sine/cosine mapping  

### 🔹 Model Training
- `HistGradientBoostingClassifier` from scikit-learn  
- Train/test split with stratification  

### 🔹 Prediction & Submission
- Generate predictions for test set  
- Save results in `sample_submission.csv`  
