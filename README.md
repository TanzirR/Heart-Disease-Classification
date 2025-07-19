# Heart Disease Classification Project

A comprehensive machine learning project for predicting heart disease using multiple classification algorithms. This project compares the performance of four different machine learning models to identify the most effective approach for heart disease prediction.

## 📊 Project Overview

This project implements and evaluates four machine learning algorithms for heart disease classification:
- **Random Forest** 
- **Support Vector Machine (SVM)**
- **Logistic Regression**
- **Naive Bayes**

The models are trained on a heart disease dataset and evaluated using various metrics including accuracy, precision, recall, and F1-score with cross-validation techniques.

## 🎯 Objectives

- Compare the performance of different machine learning algorithms for heart disease prediction
- Implement hyperparameter tuning using RandomizedSearchCV
- Evaluate model performance using 10-fold cross-validation
- Visualize results through confusion matrices and performance comparison charts

## 📁 Dataset

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

### Data Preprocessing
- Label encoding for categorical variables
- Feature matrix (X) and target variable (Y) separation
- Train-test split (80/20 ratio)

## 🛠️ Technologies Used

### Programming Language
- **Python 3.x**

### Libraries
- **Data Manipulation**: pandas, numpy
- **Machine Learning**: scikit-learn
- **Visualization**: matplotlib, seaborn
- **Model Evaluation**: sklearn.metrics

### Machine Learning Algorithms
1. **Random Forest Classifier**
   - Hyperparameter tuning with RandomizedSearchCV
   - Optimized parameters for best performance
   
2. **Support Vector Machine (Linear)**
   - Linear kernel implementation
   - Cross-validation evaluation
   
3. **Logistic Regression**
   - Maximum iteration limit: 1000
   - Random state for reproducibility
   
4. **Gaussian Naive Bayes**
   - Probabilistic classification approach

## 📈 Results

🔁 5-Fold Cross Validation

<img width="375" height="364" alt="cv 5 fold" src="https://github.com/user-attachments/assets/0737d33d-438a-4668-9eec-eabf5490af19" />

<img width="475" height="464" alt="accuracy 5 fold" src="https://github.com/user-attachments/assets/f729e728-dd23-4a9b-b873-320243b69eed" />


| Model              | Accuracy (%) | Precision | Recall | F1 Score |
|-------------------|--------------|-----------|--------|----------|
| Random Forest      | 84.00        | 0.84      | 0.86   | 0.85     |
| Logistic Regression| 80.61        | 0.85      | 0.81   | 0.82     |
| Naive Bayes        | 83.11        | 0.86      | 0.84   | 0.84     |
| SVM                | 81.70        | 0.85      | 0.82   | 0.83     |

### 🔁 10-Fold Cross Validation

<img width="375" height="364" alt="cv 10 fold" src="https://github.com/user-attachments/assets/85b6c6e9-0c61-4017-b5f0-d4a21f1e804b" />

<img width="475" height="464" alt="accuracy 10 fold" src="https://github.com/user-attachments/assets/3888b112-a5af-4649-83ee-90e5ced3f51f" />


| Model              | Accuracy (%) | Precision | Recall | F1 Score |
|-------------------|--------------|-----------|--------|----------|
| Random Forest      | **85.28**    | 0.85      | 0.88   | 0.87     |
| Logistic Regression| 83.00        | 0.85      | 0.84   | 0.84     |
| Naive Bayes        | 84.50        | 0.87      | 0.86   | 0.86     |
| SVM                | 83.32        | 0.85      | 0.85   | 0.85     |

### Key Findings
- **Random Forest** achieved the highest accuracy at 85.28%
- All models performed well with accuracies above 83%
- Random Forest showed the best balance of precision, recall, and F1-score
- Hyperparameter tuning improved Random Forest performance

## 🔧 Installation & Setup

### Prerequisites
```bash
pip install numpy pandas matplotlib scikit-learn
```

### Running the Project
1. Clone this repository:
```bash
git clone https://github.com/TanzirR/Heart-Disease-Classification.git
cd Heart-Disease-Classification
```

2. Ensure you have the `heart.csv` dataset in the project directory

3. Open and run the Jupyter notebook:
```bash
jupyter notebook "CSE 445 Heart Disease Classification.ipynb"
```

## 📊 Features

### Model Evaluation Metrics
- **Accuracy Score**: Overall correctness of predictions
- **Confusion Matrix**: Detailed breakdown of predictions vs actual
- **Precision**: True positive rate
- **Recall**: Sensitivity measure
- **F1-Score**: Harmonic mean of precision and recall
- **Cross-Validation**: 10-fold CV for robust evaluation

### Hyperparameter Tuning
- **RandomizedSearchCV** implementation for Random Forest
- Grid search across multiple hyperparameters:
  - n_estimators: [200, 400, 600, 800, 1000, 1200, 1400, 1600, 1800, 2000]
  - max_depth: [10, 20, 30, 40, 50, 60, 70, 80, 90, 100, None]
  - min_samples_split: [2, 5, 10]
  - min_samples_leaf: [1, 2, 4]
  - max_features: ['sqrt']
  - bootstrap: [True, False]

### Visualization
- Confusion matrix displays for all models
- Accuracy comparison bar charts
- Performance metrics comparison graphs

## 🎨 Visualizations

The project includes several visualization components:
- **Confusion Matrices**: Visual representation of model predictions
- **Performance Comparison Charts**: Bar plots comparing model accuracies
- **Cross-Validation Results**: Detailed performance metrics across all models

## 📝 Project Structure

```
├── CSE 445 Heart Disease Classification.ipynb    # Main notebook file
├── heart.csv                                      # Dataset (not included)
├── README.md                                      # Project documentation
└── requirements.txt                               # Dependencies (if needed)
```

## 🙏 Acknowledgments

1. Mohan, S., Thirumalai, C., & Srivastava, D. G. (2019). *Effective Heart Disease Prediction Using Hybrid Machine Learning Techniques*, IEEE Access.  
2. World Health Organization – [Cardiovascular Diseases](https://www.who.int/health-topics/cardiovascular-diseases#tab=tab_1)  
3. [Kaggle Heart Failure Dataset](https://www.kaggle.com/fedesoriano/heart-failure-prediction)


## 📞 Contact

For questions or suggestions, please open an issue in this repository.

- **GitHub:** [TanzirR](https://github.com/TanzirR)
- **Email:** [tanzir.razzaque@northsouth.edu](mailto:tanzir.razzaque@northsouth.edu)
---

**Note**: This project is for educational purposes and should not be used as a substitute for professional medical diagnosis.
