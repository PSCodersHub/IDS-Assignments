# 📄Assignment 5 - Classification & Clustering on IRIS Dataset

🔗 **Google Colab Link:**
[https://colab.research.google.com/drive/1qV3Z6O4L4uRJrzrUUmSqAMwZGb2LNWB_?usp=sharing](https://colab.research.google.com/drive/1qV3Z6O4L4uRJrzrUUmSqAMwZGb2LNWB_?usp=sharing)

---

## 📌 Project Overview

This assignment implements **Classification and Clustering** techniques on the classic **IRIS dataset** using Python and scikit-learn.
The purpose is to understand how machine learning algorithms work in practice and to compare their performance.

The dataset contains **150 samples** of iris flowers with **4 features**:

* Sepal length
* Sepal width
* Petal length
* Petal width

The target variable has **3 classes**:

* Setosa
* Versicolor
* Virginica

---

## 🧠 Algorithms Used

### 1. **Gaussian Naïve Bayes Classifier**

* A probabilistic classifier based on Bayes’ theorem.
* Assumes independence between features.
* Used here for classification of iris species.

### 2. **K-Nearest Neighbors (KNN) Classifier**

* A non-parametric classifier.
* Classifies data based on closest neighbors in feature space.
* K is set to **7**.

### 3. **K-Means Clustering**

* An unsupervised learning algorithm.
* Groups data into **clusters** based on similarity.
* Used here on a randomly generated 2D dataset.
* Also uses an **Elbow curve** to visualize optimal cluster count.

---

## 🛠️ Project Structure

The project contains three main sections:

### 📌 Section 1 — Gaussian Naïve Bayes Classification

✔ Load IRIS dataset
✔ Split data into training and test sets
✔ Train Gaussian Naïve Bayes model
✔ Predict and calculate accuracy

**Output:**

* Model accuracy displayed in percentage.

---

### 📌 Section 2 — KNN Classification

✔ Load IRIS dataset
✔ Split data
✔ Create KNN model (`n_neighbors=7`)
✔ Predict test set labels

**Output:**

* Predicted class values printed.

---

### 📌 Section 3 — K-Means Clustering + Elbow Method

✔ Generate random 2D points
✔ Fit KMeans model
✔ Compute and print cluster centers and labels
✔ Plot and display Elbow graph showing inertia values
✔ Helps decide optimal number of clusters

---

## 💡 How to Run

Make sure you have the following Python libraries installed:

```bash
pip install numpy pandas matplotlib scikit-learn
```

Then run the script in a Python environment or upload to **Google Colab** using the shared link above.

---

## 📊 Expected Results

* **Naïve Bayes** should achieve high accuracy (>90%) on this simple dataset.
* **KNN Predictions** will list predicted target labels for test samples.
* **Elbow Curve** graph will show decreasing WCSS values and help identify the best k.

---

## 📝 Notes

✔ The IRIS dataset is loaded multiple times in separate sections intentionally
✔ This makes each part **independent and complete**
✔ Commented code explains each line for clarity and grading

---

## 🎯 Learning Outcomes

By completing this assignment, you will:

* Understand how classification algorithms work
* Know how to implement Naïve Bayes and KNN in Python
* Learn the concept of clustering and the Elbow method
* Practice splitting data and evaluating model performance

---

## 📚 References

* scikit-learn documentation: [https://scikit-learn.org](https://scikit-learn.org)
* IRIS dataset info: [https://archive.ics.uci.edu/ml/datasets/Iris](https://archive.ics.uci.edu/ml/datasets/Iris)

---

## Author

***Priyanshu Sahoo***

---
---


<div align="center"> <h1 style=font-weight: bold;>@PSCodersHub</h1> </div>
