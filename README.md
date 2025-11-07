# Titanic Survival Prediction

This project is my first end-to-end machine learning model built using the classic **Titanic dataset** from Kaggle.  
The goal is to predict whether a passenger survived the Titanic disaster based on demographic and ticket-related features.

---

## Project Overview
This project focuses on:
- Data cleaning and handling missing values  
- Feature engineering (creating new columns like `FamilySize` and `IsAlone`)  
- Encoding categorical features (`Sex`, `Embarked`)  
- Training a **Random Forest Classifier** to predict survival outcomes  
- Generating a submission file for Kaggle evaluation  

My first submission achieved a score of **0.75 accuracy** on Kaggle.

---

## Dataset
The dataset comes from the [Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic) competition on Kaggle.

- `train.csv` — used for training and validation  
- `test.csv` — used for prediction and submission  
- `submission.csv` — model output file containing predictions

---

## Features Used
- **Pclass** – Passenger class (1st, 2nd, 3rd)  
- **Sex** – Gender (encoded as 0/1)  
- **Age** – Filled missing values with mean age  
- **SibSp** – Number of siblings/spouses aboard  
- **Parch** – Number of parents/children aboard  
- **Fare** – Passenger fare  
- **Embarked** – Port of embarkation (encoded numerically)  
- **FamilySize** – Created from `SibSp + Parch + 1`  
- **IsAlone** – 1 if passenger is alone, 0 otherwise  

---

## Model
I used a **Random Forest Classifier** from Scikit-learn.

Steps:
1. Preprocessed the data (handled missing values and encoding)
2. Engineered new features
3. Trained the Random Forest model on the training data
4. Generated predictions on the test data
5. Saved the output as `submission.csv` for Kaggle submission

---

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
---

## Next Steps
- Extract titles from names for additional predictive power  
- Create bins for Age and Fare to capture non-linear patterns  
- Experiment with XGBoost and hyperparameter tuning  
- Implement a Pipeline for consistent preprocessing  

---

## Repository Structure
