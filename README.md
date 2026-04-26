# In-Vehicle-Coupon-Recommendation-System

## Project Overview
This project aims to predict whether a driver will accept a coupon while driving, based on contextual, behavioral, and demographic features.

The objective is to build a machine learning model that helps businesses improve targeted marketing by recommending coupons more effectively.

## Dataset Description
The dataset is based on survey responses collected via Amazon Mechanical Turk. Each row represents a driving scenario where a user is offered a coupon and chooses whether to accept it.

## Dataset Details:
- Total Records: 12,684
- Features: 25
- Target Variable: `Y` (Coupon Acceptance)

## Target Variable:
- `1` → Coupon accepted  
- `0` → Coupon rejected  

## Features Included

## Contextual Features
- `destination` – Home, Work, No Urgent Place
- `passenger` – Alone, Friend(s), Partner, Kid(s)
- `weather` – Sunny, Rainy, Snowy
- `temperature` – Outside temperature
- `time` – Time of day

## Coupon Features
- `coupon` – Type of coupon (Coffee House, Restaurant, Bar, etc.)
- `expiration` – Time before coupon expires

## Problem Statement
Businesses often send coupons without personalization, leading to low acceptance rates.

This project solves a **binary classification problem** to predict whether a user will accept a coupon, enabling better targeting and improved engagement.

## Tech Stack
- Python
- Pandas, NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Data Loading and Understanding  
2. Exploratory Data Analysis (EDA)  
3. Data Cleaning & Handling Missing Values  
4. Encoding Categorical Features  
5. Train-Test Split  
6. Model Training  
7. Model Evaluation
   
## Model Implementation

A **Decision Tree Classifier** was used to build the prediction model.

## Splitting Criteria Used:
- Gini Index
- Entropy (Information Gain)

Both were evaluated to understand how impurity measures affect model performance.

## Model Performance

- Model: Decision Tree Classifier  
- Criteria: Gini & Entropy  
- Accuracy: 0.68

## Observations

- The model captures non-linear relationships between features such as:
  - Coupon type
  - Time of day
  - User behavior patterns (e.g., coffee house visits)
- Overfitting was observed when tree depth was not controlled
- Performance indicates that user decision-making is influenced by multiple interacting factors
