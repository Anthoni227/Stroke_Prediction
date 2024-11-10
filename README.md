# Stroke Prediction Project

## Overview
This project predicts stroke likelihood based on various health and lifestyle factors using machine learning models. Identifying stroke risk early enables preventive measures to improve healthcare outcomes.

## Models and Performance
Below is a summary of each model's performance metrics, with **Random Forest Classifier** emerging as the top performer.

### Model Performance Table

| **Model**                | **Accuracy** | **Precision** | **Recall** | **F1 Score** |
|--------------------------|--------------|---------------|------------|--------------|
| Logistic Regression      | 91.0%        | 0.91          | 0.90       | 0.91         |
| Gaussian Naive Bayes     | 84.0%        | 0.77          | 0.98       | 0.86         |
| Decision Tree Classifier | 90.0%        | 0.88          | 0.93       | 0.90         |
| Random Forest Classifier | 98.0%        | 0.98          | 0.99       | 0.98         |
| XGBoost Classifier       | 96.0%        | 0.94          | 0.97       | 0.96         |
| AdaBoost Classifier      | 91.0%        | 0.90          | 0.93       | 0.91         |

### Highlights of Model Performance

- **Random Forest Classifier**: Best-performing model with an impressive **98.0% accuracy**, **98.0% precision**, and **99.0% recall**, indicating its robustness in classifying both positive and negative stroke cases.
- **XGBoost Classifier**: Achieved **96.0% accuracy**, **94.0% precision**, and **97.0% recall**, making it highly effective in identifying stroke risks.
- **Decision Tree Classifier**: Performed well with **90.0% accuracy**, though slightly lower than ensemble methods.
- **Logistic Regression**: A reliable model with **91.0% accuracy**, though slightly less optimal than tree-based models in precision and recall.
- **AdaBoost Classifier**: Matched Logistic Regression with **91.0% accuracy**, showing good performance, but slightly outperformed by Random Forest and XGBoost.
- **Gaussian Naive Bayes**: Least effective with **84.0% accuracy**, demonstrating high recall but low precision, indicating it tends to overpredict positive cases.

## Project Structure

### Data Preprocessing
- **Handling Missing Values**: Managed missing values to ensure clean data.
- **Feature Encoding**: Encoded categorical variables for model compatibility.
- **Scaling**: Scaled numerical features to improve model performance.

### Model Training and Evaluation
- Built and trained models using Scikit-Learn with hyperparameter tuning via GridSearchCV.
- Evaluated models based on accuracy, precision, recall, F1 Score, and AUC-ROC curve.

## Installation and Requirements

### Prerequisites
- Python 3.8+
- Jupyter Notebook or any IDE supporting Python

### Dependencies
Install dependencies with:

```bash
pip install -r requirements.txt

### Conclusions 
The models provided valuable insights into predicting Stroke Prediction, with **Random Forest** being the most reliable. 
