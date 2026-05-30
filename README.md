# WDBC Breast Cancer Classification

## 1. Project Title

WDBC Breast Cancer Classification using Multiple Machine Learning Classifiers

---

## 2. Project Purpose

The purpose of this project is to classify breast cancer tumors as malignant or benign using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset.

The project trains and compares multiple machine learning classifiers, evaluates their performance, identifies the best-performing classifier, and visualizes the results using confusion matrices and scatter plots.

---

## 3. Dataset Used

Dataset: Wisconsin Diagnostic Breast Cancer (WDBC)

Source: Scikit-learn built-in dataset

```python
from sklearn import datasets
wdbc = datasets.load_breast_cancer()
```

Dataset Information:

* Samples: 569
* Features: 30 numeric features
* Classes: malignant, benign

---

## 4. How to Install Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```

---

## 5. How to Run the Code

This project was developed and tested with Python 3.10.19.

Open and run the Jupyter Notebook:

```bash
jupyter notebook wdbc_classification.ipynb
```

The notebook performs the following tasks:

1. Loads the WDBC dataset.
2. Trains a default SVM classifier using the entire dataset (`X`, `y`) and manually calculates Accuracy, Precision, and Recall.
3. Splits the dataset into training and testing sets (80:20).
4. Trains and compares the following classifiers using the train/test split:

   * SVM
   * Decision Tree
   * KNN
   * Random Forest
5. Identifies the classifier with the highest test accuracy.
6. Generates visualization files.

---

## 6. Output Files

### wdbc_classification_matrix.png

A 2×2 visualization containing the confusion matrices for:

* SVM
* Decision Tree
* KNN
* Random Forest

### wdbc_classification_scatter.png

A 2×2 visualization containing scatter plots for:

* SVM
* Decision Tree
* KNN
* Random Forest

---

## 7. Best Classifier Result

The program automatically compares classifier accuracies and reports:

* Best Classifier
* Best Accuracy

Example result from one execution:

* Best Classifier: Random Forest
* Best Accuracy: 0.9649
