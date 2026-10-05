# Task 1: Iris Flower Classification

## Problem Statement

The Iris flower dataset is a classic dataset in machine learning and statistics. The goal is to classify iris flowers into three species (Setosa, Versicolor, and Virginica) based on four features: sepal length, sepal width, petal length, and petal width.

## Dataset

The Iris dataset contains 150 samples:
- 50 samples of each species
- 4 features per sample (all in centimeters):
  - Sepal length
  - Sepal width
  - Petal length
  - Petal width

The dataset is included in scikit-learn, so no external download is required.

## Approach

1. **Data Loading & Exploration**
   - Load the Iris dataset from scikit-learn
   - Display basic statistics and information
   - Check for missing values

2. **Exploratory Data Analysis (EDA)**
   - Visualize feature distributions
   - Create pair plots to identify patterns
   - Analyze correlations between features

3. **Data Preparation**
   - Split data into training (70%) and testing (30%) sets
   - Apply feature scaling using StandardScaler

4. **Model Training & Comparison**
   - Train multiple classifiers:
     - Logistic Regression
     - K-Nearest Neighbors (KNN)
     - Decision Tree
     - Random Forest
   - Compare performance on validation

5. **Model Evaluation**
   - Evaluate on the held-out test set
   - Generate confusion matrix
   - Display classification report with precision, recall, and F1-score

## Results

All models achieved excellent performance on the Iris dataset:

| Model | Test Accuracy |
|-------|---------------|
| Logistic Regression | 100.0% |
| K-Nearest Neighbors | 100.0% |
| Decision Tree | 100.0% |
| Random Forest | 100.0% |

**Best Model:** All models performed perfectly on this dataset. Random Forest was selected as the final model for its robustness and ability to handle non-linear relationships.

### Confusion Matrix

The confusion matrix for Random Forest showed perfect classification with no misclassifications across all three species.

### Classification Report

```
              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        19
  versicolor       1.00      1.00      1.00        13
   virginica       1.00      1.00      1.00        13

    accuracy                           1.00        45
   macro avg       1.00      1.00      1.00        45
weighted avg       1.00      1.00      1.00        45
```

## Key Findings

1. The Iris dataset is linearly separable for Setosa, making it easy to classify
2. Versicolor and Virginica show some overlap but remain distinguishable
3. Petal measurements (length and width) are stronger predictors than sepal measurements
4. All models achieved perfect accuracy, indicating the dataset's simplicity

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open `iris_classification.ipynb` and run all cells

## Files

- `iris_classification.ipynb` - Main notebook with analysis and code
- `requirements.txt` - Python dependencies
- `README.md` - This file

## Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation
- **numpy** - Numerical operations
- **matplotlib & seaborn** - Data visualization
- **scikit-learn** - Machine learning models and metrics

## Author

**Théodore Dorvi**
- GitHub: [@Thedy09](https://github.com/Thedy09)
