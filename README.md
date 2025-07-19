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

The project uses the `heart.csv` dataset containing various medical indicators and patient information to predict heart disease occurrence.

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

### Model Performance (10-Fold Cross Validation)

| Model | Accuracy (%) |
|-------|-------------|
| Random Forest | 85.28 |
| Naive Bayes | 84.50 |
| SVM | 83.32 |
| Logistic Regression | 83.00 |

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
git clone [your-repository-url]
cd heart-disease-classification
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

## 🚀 Future Improvements

- Implement additional algorithms (XGBoost, Neural Networks)
- Feature importance analysis
- ROC curve analysis and AUC scores
- Ensemble methods combining multiple models
- Deep learning approaches
- Real-time prediction interface

## 👥 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📜 License

This project is available under the MIT License. See LICENSE file for more details.

## 🙏 Acknowledgments

- Dataset providers for the heart disease dataset
- Scikit-learn community for excellent machine learning tools
- Contributors to the open-source libraries used in this project

## 📞 Contact

For questions or suggestions, please open an issue in this repository.

---

**Note**: This project is for educational purposes and should not be used as a substitute for professional medical diagnosis.
