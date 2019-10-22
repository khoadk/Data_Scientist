# Breast Cancer Detection

## 1. Project Description:
- Breast cancer (BC) is one of the most common cancers among women worldwide, representing the majority of new cancer cases and cancer-related deaths according to global statistics, making it a significant public health problem in today’s society. The early diagnosis of BC can improve the prognosis and chance of survival significantly, as it can promote timely clinical treatment to patients.
- Detecting breast cancer through machine learning models such as **LogisticRegression, KNeighborsClassifier and SVC...**

## 2. Datasets:

Source: https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(original)

Attribute Information:

1. Sample code number: id number
2. Clump Thickness: 1 - 10
3. Uniformity of Cell Size: 1 - 10
4. Uniformity of Cell Shape: 1 - 10
5. Marginal Adhesion: 1 - 10
6. Single Epithelial Cell Size: 1 - 10
7. Bare Nuclei: 1 - 10
8. Bland Chromatin: 1 - 10
9. Normal Nucleoli: 1 - 10
10. Mitoses: 1 - 10
11. Class: (2 for benign, 4 for malignant)

## 3. Making predictions and evaluating performance
- We will now evaluate our model on the test set with respect to classification accuracy. But we will also take a look the model's confusion matrix.

- In the case of predicting breast cancer. **it is more important to see if our machine learning model is able to correctly predict the 'malignant' group.**
- **LogisticRegression** model:
    - False to predict maligrant is **8.62%**
    - True to predict maligrant is **91.38%**
    - Best Accuracy: **96.7%** using {'logreg__max_iter': 100, 'logreg__tol': 0.01}
- **SVC** model: 
    - False to predict maligrant is **1.72%**
    - True to predict maligrant is **98.28%**
    - Best Accuracy: **95.6%** using {'SVM__C': 1}
- **KNN** model:
    - False to predict maligrant is **8.62%**
    - True to predict maligrant is **91.38%**
    - Best: **96.7%** using {'KNN__n_neighbors': 7}
