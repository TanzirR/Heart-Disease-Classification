# Heart Disease Classification using Machine Learning

This project evaluates the performance of multiple machine learning classification models in predicting heart disease using a real-world dataset. Implemented and compared four popular models: **Random Forest**, **Support Vector Machine (SVM)**, **Logistic Regression**, and **Naive Bayes**.

## 📊 Objective

To identify the best-performing machine learning model for heart disease classification based on key evaluation metrics such as accuracy, precision, recall, and F1 score.

## 👩‍⚕️ Dataset

- Source: [Kaggle - Heart Failure Prediction](https://www.kaggle.com/fedesoriano/heart-failure-prediction)
- Total Instances: 918
- Features: 11 clinical features including:
  - Age
  - Sex
  - Chest Pain Type
  - Resting Blood Pressure
  - Cholesterol
  - Fasting Blood Sugar
  - Resting ECG
  - Max Heart Rate
  - Exercise-induced Angina
  - Oldpeak
  - ST Slope
- Target: Binary classification (0 - Normal, 1 - Heart Disease)

## 🛠️ Methodology

- **Tools & Libraries**: Python 3.9.0, Scikit-learn, Matplotlib, Jupyter Notebook
- **Data Split**: 80% Training, 20% Testing
- **Validation Techniques**:
  - 5-Fold Cross Validation
  - 10-Fold Cross Validation
- **Metrics Evaluated**: Accuracy, Precision, Recall, F1 Score, Confusion Matrix
- **Hyperparameter Tuning**: Randomized Search CV (for Random Forest)

## 📈 Results

### 🔁 5-Fold Cross Validation

| Model              | Accuracy (%) | Precision | Recall | F1 Score |
|-------------------|--------------|-----------|--------|----------|
| Random Forest      | 84.00        | 0.84      | 0.86   | 0.85     |
| Logistic Regression| 80.61        | 0.85      | 0.81   | 0.82     |
| Naive Bayes        | 83.11        | 0.86      | 0.84   | 0.84     |
| SVM                | 81.70        | 0.85      | 0.82   | 0.83     |

### 🔁 10-Fold Cross Validation

| Model              | Accuracy (%) | Precision | Recall | F1 Score |
|-------------------|--------------|-----------|--------|----------|
| Random Forest      | **85.28**    | 0.85      | 0.88   | 0.87     |
| Logistic Regression| 83.00        | 0.85      | 0.84   | 0.84     |
| Naive Bayes        | 84.50        | 0.87      | 0.86   | 0.86     |
| SVM                | 83.32        | 0.85      | 0.85   | 0.85     |

> ✅ Random Forest consistently outperformed the other models in both validation settings.

## 📌 Conclusion

Random Forest yielded the highest accuracy and overall performance among all tested models for heart disease prediction. The accuracy improved further after hyperparameter tuning and using 10-fold cross validation.

## 🧑‍💻 Authors

- **Tanzir Bin Razzaque**  
  Electrical and Computer Engineering Dept., North South University  
  📧 tanzir.razzaque@northsouth.edu

## 📚 References

1. Mohan, S., Thirumalai, C., & Srivastava, D. G. (2019). *Effective Heart Disease Prediction Using Hybrid Machine Learning Techniques*, IEEE Access.  
2. World Health Organization – [Cardiovascular Diseases](https://www.who.int/health-topics/cardiovascular-diseases#tab=tab_1)  
3. [Kaggle Heart Failure Dataset](https://www.kaggle.com/fedesoriano/heart-failure-prediction)

---

