# Assignment 6 - Dimensionality Reduction using PCA and LDA

🔗 **Google Colab Notebook:**
[https://colab.research.google.com/drive/12knGK9AcEHoZZR0c38e05mf2lkcami-A?usp=sharing](https://colab.research.google.com/drive/12knGK9AcEHoZZR0c38e05mf2lkcami-A?usp=sharing)

---

## Overview

This assignment demonstrates **Dimensionality Reduction techniques** used in machine learning and data science. Two popular methods are implemented:

* Principal Component Analysis (PCA)
* Linear Discriminant Analysis (LDA)

Dimensionality reduction helps simplify datasets with many features while preserving the most important information. This improves computational efficiency, visualization, and model performance.

---

## Objectives

* Understand the concept of dimensionality reduction.
* Apply PCA to reduce features in a mushroom dataset.
* Apply LDA to classify iris flower species.
* Visualize the transformed feature space.

---

## Datasets Used

### 1. Mushroom Dataset

Dataset Link:
[https://www.kaggle.com/datasets/rumeysagnaydn/mushroomcsv](https://www.kaggle.com/datasets/rumeysagnaydn/mushroomcsv)

Dataset used for applying PCA.

**Dataset Details**

| Attribute       | Description                         |
| --------------- | ----------------------------------- |
| Total Samples   | 8124                                |
| Total Features  | 23                                  |
| Target Variable | Mushroom class (Edible / Poisonous) |
| Data Type       | Categorical                         |

Features include characteristics like cap shape, cap color, odor, gill color, stalk shape, habitat, etc.

---

### 2. Iris Dataset

Dataset provided by **scikit-learn** library.

This dataset contains measurements of iris flowers and is used to classify them into three species:

* Setosa
* Versicolor
* Virginica

**Dataset Details**

| Attribute | Description |
| --------- | ----------- |
| Samples   | 150         |
| Features  | 4           |
| Classes   | 3           |

---

## Methodology

### 1. Principal Component Analysis (PCA)

PCA is an unsupervised dimensionality reduction technique that transforms the original features into a new set of variables called **principal components**. These components capture the maximum variance present in the dataset.

Steps performed:

1. Load the mushroom dataset.
2. Encode categorical variables into numeric values.
3. Standardize the dataset.
4. Apply PCA.
5. Visualize variance explained by each principal component.
6. Plot the reduced dimensional representation.

---

### 2. Linear Discriminant Analysis (LDA)

LDA is a supervised dimensionality reduction technique that finds the linear combinations of features that best separate multiple classes.

Steps performed:

1. Load the iris dataset.
2. Separate features and labels.
3. Train the LDA model.
4. Evaluate the model using cross-validation.
5. Predict class for a new observation.
6. Visualize the LDA transformed space.

---

## Results

### PCA Results

* PCA reduced the dimensionality of the mushroom dataset.
* The variance plot showed how much information each component retains.
* Dimensionality reduction helped visualize feature importance.

### LDA Results

* LDA successfully separated the iris species.
* Cross-validation accuracy was approximately **98%**.
* The scatter plot clearly displayed distinct clusters for each flower species.

---

## Conclusion

PCA and LDA are powerful dimensionality reduction techniques used in machine learning.

PCA focuses on maximizing variance in the dataset without considering class labels, making it useful for exploratory data analysis and feature reduction.

LDA, on the other hand, maximizes the separation between classes and is commonly used in classification problems.

Through this assignment, both methods were successfully implemented and demonstrated using real-world datasets.

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Scikit-learn
* Google Colab

---

## Author

***Priyanshu Sahoo***

---
---

<div align="center"> <h1 style=font-weight: bold;>@PSCodersHub</h1> </div>