# **Assignment 4 – Descriptive Statistics & Power Transformation (Diabetes Dataset)**

## 📌 **Google Colab Link:**
🔗 [https://colab.research.google.com/drive/1j93CM43YCyz88cQr7ahY34B4KnQbJpu_?usp=sharing](https://colab.research.google.com/drive/1j93CM43YCyz88cQr7ahY34B4KnQbJpu_?usp=sharing)

---

## 📘 **1. Introduction**

This assignment focuses on applying **descriptive statistical analysis** and **power transformation** to a real regression dataset, followed by evaluation using **Linear Regression**. The primary goal is to understand how data transformation affects model performance and distribution characteristics.

The practice section uses the *Iris dataset* to build familiarity with descriptive statistics. The main assignment uses the *Diabetes dataset*, which is a standard regression dataset available in scikit-learn.

---

## 🧠 **2. Dataset Description**

### Practice Dataset

* **Iris Dataset**

  * Contains 150 samples of three flower species.
  * Used for practice only (classification dataset).

### Main Dataset

* **Diabetes Dataset**

  * A regression dataset containing clinical measurements and a target disease progression metric.
  * Fully numerical, suitable for regression and transformation.

---

## 🛠 **3. Steps Performed**

### 🔹 Step 1 — Import Libraries

We imported essential Python libraries for:

* Data handling (`pandas`, `numpy`)
* Visualization (`matplotlib`, `seaborn`)
* Machine learning (`scikit-learn`)
* Statistical analysis (`scipy.stats`)

---

### 🔹 Step 2 — Load Dataset

The Diabetes dataset was loaded using scikit-learn’s `load_diabetes()` method and converted into a Pandas DataFrame, including the target column.

---

### 🔹 Step 3 — Handle Missing Values

Checked for null entries using `.isnull().sum()` and confirmed that the dataset contains no missing values.

---

### 🔹 Step 4 — Descriptive Statistics

Used `.describe()` to compute:

* Mean
* Standard deviation
* Minimum, maximum
* Quartiles

This helps understand general data behavior before modeling.

---

### 🔹 Step 5 — Train-Test Split

Split features and target into:

* **Training set (67%)**
* **Testing set (33%)**

This is standard practice to evaluate model performance on unseen data.

---

### 🔹 Step 6 — Linear Regression (Before Transformation)

Performed a baseline Linear Regression:

```python
lr = LinearRegression()
lr.fit(X_train, y_train)
```

Calculated R² score to measure initial model performance:

```
R² before transformation: 0.5192
```

---

### 🔹 Step 7 — Check Data Distribution

Plotted:

* Histogram
* Probability plot (Q-Q plot)

for each feature to understand normality and skewness.

---

### 🔹 Step 8 — Power Transformation

Applied **Yeo-Johnson** transformation:

```python
pt = PowerTransformer(method='yeo-johnson')
```

This method was chosen because:

* It handles both positive and negative values.
* It improves normality of features.
* It is more flexible than Box-Cox in real regression datasets.

---

### 🔹 Step 9 — Linear Regression (After Transformation)

Trained the model again using transformed data and calculated new performance:

```
R² after transformation: 0.5049
```

---

### 🔹 Step 10 — Compare Before & After

Plotted distributions before and after transformation to confirm improvement in data normality visually.

---

## 📊 **4. Results**

| Metric                         | Value      |
| ------------------------------ | ---------- |
| R² before transformation       | **0.5192** |
| R² after Yeo-Johnson transform | **0.5049** |

---

## 📌 **5. Interpretation and Conclusion**

* The **baseline Linear Regression** showed moderate performance with an R² of ~0.52.
* After applying **Yeo-Johnson power transformation**, the model performance **slightly decreased** (R² ~0.50).
* This outcome shows that **power transformation does not always improve predictive performance**, but it does help make feature distributions more normal.
* Since the dataset has **zero and negative values**, Yeo-Johnson was the appropriate transformation method rather than Box-Cox.
* Visual distribution plots before and after transformation confirm improved symmetry and reduced skewness in the features.

---

## 🧾 **6. Key Learnings**

1. **Descriptive statistics** provide a deep understanding of feature behavior.
2. **Power transformations** such as Yeo-Johnson help improve feature normality.
3. **Model evaluation metrics** (like R²) help compare model performance objectively.
4. Real-world transformation may not always increase accuracy but often makes model assumptions more valid.
5. It is important to choose the correct **power transformation** method based on data characteristics.

---

## 🎓 **7. Conclusion**

> This assignment demonstrated the full workflow of regression analysis with transformation. After exploring descriptive statistics and applying Yeo-Johnson transformation, it was concluded that while transformation improved data normality, it did not enhance model performance in this case. However, it remains an important tool for satisfying mathematical assumptions of regression models.

---
---

<div align="center"> <h1 style=font-weight: bold;>@PSCodersHub</h1> </div>