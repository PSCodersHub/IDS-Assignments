# Assignment 3 – Logistic Regression & Multi-class ROC on Iris Dataset

## 📌 Project Title

**Multi-Class Classification on the Iris Dataset Using Logistic Regression**

## 📌 Colab Notebook Link

🔗 [https://colab.research.google.com/drive/1oaZ8SuoBELnsj-IXuVBlP3eFc3GwvhHG?usp=sharing](https://colab.research.google.com/drive/1oaZ8SuoBELnsj-IXuVBlP3eFc3GwvhHG?usp=sharing)

---

## 📗 Objective

The goal of this project is to:

1. Load and explore the **Iris dataset**
2. Perform **data preprocessing**
3. Train and evaluate a **Logistic Regression classifier**
4. Generate **confusion matrix**, **accuracy**, and **ROC curves**
5. Illustrate **AUROC for multi-class classification**

---

## 📘 Dataset Description

The **Iris dataset** is a well-known benchmark dataset with:

* 150 samples
* 4 features:

  * Sepal Length
  * Sepal Width
  * Petal Length
  * Petal Width
* 3 classes (species):

  * 0: *Iris-setosa*
  * 1: *Iris-versicolor*
  * 2: *Iris-virginica*

The dataset is imported directly from `sklearn.datasets`.

---

## 🧠 Tools and Libraries Used

| Library                   | Purpose                       |
| ------------------------- | ----------------------------- |
| `numpy`, `pandas`         | Data handling                 |
| `sklearn.preprocessing`   | Label encoding & binarization |
| `sklearn.model_selection` | Train-test splitting          |
| `sklearn.linear_model`    | Logistic Regression           |
| `sklearn.multiclass`      | One-Vs-Rest classifier        |
| `sklearn.metrics`         | Confusion matrix, ROC, AUC    |
| `matplotlib`              | Plotting ROC curves           |

---

## 🧾 Step-by-Step Explanation

### 1. Import Libraries

All necessary Python packages are imported including sklearn modules.

> **Note:** Some imports like `LinearRegression`, `cross_val_score`, and `PowerTransformer` were included but not used in the model — these are not required for this experiment.

---

### 2. Load and Prepare Dataset

The Iris dataset is loaded using `load_iris()` and converted into a pandas DataFrame with meaningful column names.

The target labels are encoded using `LabelEncoder` to demonstrate label encoding, although the dataset target labels are already numeric.

---

### 3. Train-Test Split

The dataset is split using `train_test_split()` to create training and testing subsets.

---

### 4. Train Logistic Regression Model

A Logistic Regression classifier is trained on the training data and used to predict class labels on the test set.

---

### 5. Model Evaluation

The following metrics are computed:

* **Confusion Matrix**
* **Accuracy**
* (Note: `r2_score` is shown but classification metrics like accuracy are more appropriate.)

---

### 6. ROC Curve for Multi-Class

ROC analysis is done using:

* `OneVsRestClassifier` strategy
* Binarized labels with `label_binarize()`
* `roc_curve()` and `auc()` for each class

The ROC curves are plotted for all three classes with AUC values indicated in the legend.

---

## 📌 What is NOT Required (but included in the code)

| Part                      | Reason                              |
| ------------------------- | ----------------------------------- |
| `LinearRegression`        | Not relevant for classification     |
| `cross_val_score`         | Not used                            |
| `PowerTransformer`        | Not applied                         |
| `plot_roc_curve()` helper | Not used for multi-class ROC        |
| `r2_score`                | Used for regression, not ideal here |

These can be mentioned in your comments as “included for demonstration but not required for the results.”

---

## 🖼 Results & Output

The notebook produces:

✅ A confusion matrix
✅ Model accuracy
✅ Multi-class ROC plot with AUC for:

* Class 0
* Class 1
* Class 2

Each ROC curve displays how well the classifier distinguishes one class versus all others.

---

## 📌 Conclusion

This experiment successfully applies Logistic Regression to the Iris dataset and evaluates model performance using confusion matrix and ROC curves. The ROC plot demonstrates the classifier’s ability to distinguish between all three classes.

---

## 🧠 Viva / Oral Exam Tips

✔ Explain why ROC requires binarization for multi-class problems
✔ Clarify why `r2_score` isn’t ideal here
✔ Mention that target labels were already numeric

---
---

<div align="center"> <h1 style=font-weight: bold;>@PSCodersHub</h1> </div>

