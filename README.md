# Prediction of Road Accident Victims in Quebec

## Project Overview
This project aims to predict the number of victims involved in road accidents in Quebec using data-driven and machine learning approaches. It was conducted as part of the **IND6212 - Industrial Data Exploration** course at Polytechnique Montréal.

---

## Objectives
1. **Analyze accident data** from Quebec to identify significant patterns and factors influencing road safety.
2. **Prepare and preprocess data** to ensure it is clean and suitable for machine learning models.
3. **Develop a predictive model** to estimate the number of accident victims based on relevant explanatory variables.
4. **Evaluate the model's performance** using metrics such as Mean Squared Error (MSE) and R² score.

---

## Data Source
The dataset was obtained from [Données Québec](https://donneesquebec.ca), specifically from the Société de l'assurance automobile du Québec (SAAQ). It includes **108,185 records** of road accidents from 2022, with **25 explanatory variables**, such as:
- **Road conditions** (dry, wet, snowy).
- **Weather conditions** (clear, rainy, foggy).
- **Accident details** (time, region, severity, number of vehicles involved).
- **Traffic and road attributes** ( speed limits, road configuration).

---

### Predictive Model
- **Algorithm**: Random Forest Regressor
  - Chosen for its ability to handle large datasets with mixed categorical and numerical features.
  - Known for its robustness against overfitting and ability to generalize well.
- **Hyperparameter Tuning**: Performed using **Grid Search** with **cross-validation (3-fold)** to optimize:
  - `max_depth`: Maximum depth of the trees.
  - `min_samples_split`: Minimum samples to split a node.
  - `min_samples_leaf`: Minimum samples in a leaf node.

### Model Evaluation
The model's performance was assessed using:
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Error (MAE)**
- **R² Score**

---

## Results
### Model Performance
- **Training Set**:
  - MSE: 0.0543
  - R²: 0.8439
- **Test Set**:
  - MSE: 0.0589
  - RMSE: 0.2428
  - MAE: 0.0803
  - R²: 0.8275

The model demonstrated strong predictive capabilities, with an R² score of 82.75%, indicating that it effectively explains most of the variance in the number of victims.

## Authors
- **David De Blas**
- **Yassine Azrou**
- **Yannis Redjah**
