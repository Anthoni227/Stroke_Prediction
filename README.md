# 🧠 Stroke Prediction Project 🚑

## 📊  Overview
This project predicts the likelihood of a stroke based on various health and lifestyle factors using machine learning models. Identifying stroke risk early enables preventive measures to improve healthcare outcomes.

## 🗂️ Project Workflow
![stroke_workflow](https://github.com/user-attachments/assets/938f2e19-a3bc-4db6-b2c0-32dcd45738bd)

### 🧹 Data Preprocessing
- **🔍 Handling Missing Values**: Missing data was addressed to maintain a clean dataset.
- **🔠 Feature Encoding**: Categorical variables were encoded to ensure model compatibility.
- **📏 Feature Scaling**: Numerical features were scaled to enhance model performance.
- **⚖️ Resampling Technique**: SMOTE (Synthetic Minority Over-sampling Technique) was used to handle class imbalance by oversampling the minority class.
  
### ⚙️ Model Training and Evaluation
- **🔧 Training**: Models were trained using Scikit-Learn, with hyperparameter tuning conducted via GridSearchCV.
- **📊 Evaluation**: Models were evaluated on several performance metrics, including accuracy, precision, recall, F1 score, and the AUC-ROC curve.
  
## 📈 Model Performance

Below is a summary of each model's performance metrics. The **Random Forest Classifier** emerged as the top performer.

| **Model**                | **Accuracy** | **Precision** | **Recall**  |  **F1 Score** |
|--------------------------|--------------|---------------|-------------|---------------|
| Logistic Regression      | 91.0%        | 91.0%         | 90.0%       |  91.0%        |
| Gaussian Naive Bayes     | 84.0%        | 77.0%         | 98.0%       |  86.0%        |
| Decision Tree Classifier | 90.0%        | 88.0%         | 93.0%       |  90.0%        |
| Random Forest Classifier | 98.0%        | 98.0%         | 99.0%       |  98.0%        |
| XGBoost Classifier       | 96.0%        | 94.0%         | 97.0%       |  96.0%        |
| AdaBoost Classifier      | 91.0%        | 90.0%         | 93.0%       |  91.0%        |

### 🔑 Key Insights

- **Random Forest Classifier**: Best performer with **98.0% accuracy**, **98.0% precision**, and **99.0% recall**, excelling in both identifying true positives and negatives.
- **XGBoost Classifier**: A close second with **96.0% accuracy**, **94.0% precision**, and **97.0% recall**, demonstrating strong performance in stroke prediction.
- **Decision Tree Classifier**: Showed good results with **90.0% accuracy**, though not as robust as ensemble methods like Random Forest or XGBoost.
- **Logistic Regression**: A reliable model at **91.0% accuracy**, but slightly less optimal than tree-based models in precision and recall.
- **AdaBoost Classifier**: Matched Logistic Regression in **accuracy** (91.0%) but slightly lagged behind in performance compared to Random Forest and XGBoost.
- **Gaussian Naive Bayes**: Performed the least with **84.0% accuracy**, highlighting its tendency to overpredict positive cases (high recall but low precision).

### 📚 Conclusion
The models provided valuable insights into predicting the likelihood of a stroke. Among them, **Random Forest** stood out as the most reliable model, delivering the highest accuracy(98%) and recall. This makes it a strong candidate for deployment in stroke prediction systems, potentially aiding in early diagnosis and preventive healthcare measures.

