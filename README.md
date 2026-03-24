# 🌸 Iris Classification

A machine learning project that classifies iris flowers into three species — *Setosa*, *Versicolor*, and *Virginica* — using sepal and petal measurements.

---

## 📌 Overview

The [Iris dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html) is one of the most well-known datasets in machine learning. This project explores the dataset through exploratory data analysis (EDA), trains multiple classification models, and evaluates their performance.

**Goal:** Predict the iris species from four features:
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

---

## 🛠️ Technologies Used

| Category | Tools |
|---|---|
| Language | Python 3.x |
| Data manipulation | pandas, NumPy |
| Visualization | matplotlib, seaborn |
| Machine learning | scikit-learn |
| Notebook | Jupyter Notebook |

---

## 📂 Project Structure

```
iris-classification/
├── data/
│   └── iris.csv
├── notebooks/
│   └── iris_classification.ipynb
├── src/
│   └── model.py
├── requirements.txt
└── README.md
```

---

## 🔍 Exploratory Data Analysis

- Pairplot of all four features colored by species
- Correlation heatmap
- Distribution plots per feature and species
- Box plots to identify separability

Key finding: **Petal length and petal width** are the most discriminative features, showing clear separation between *Setosa* and the other two species.

---

## 🤖 Models & Results

The following classifiers were trained and evaluated using 80/20 train-test split and 5-fold cross-validation:

| Model | Test Accuracy |
|---|---|
| Logistic Regression | 97.0% |
| K-Nearest Neighbors | 96.7% |
| Decision Tree | 96.7% |
| Random Forest | **98.0%** |
| Support Vector Machine | 97.3% |

**Best model: Random Forest** with 98.0% accuracy.

Evaluation metrics used: accuracy, precision, recall, F1-score, confusion matrix.

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Run the notebook

```bash
jupyter notebook notebooks/iris_classification.ipynb
```

### Run the model script

```bash
python src/model.py
```

---

## 📊 Sample Output

```
Classification Report:
              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        10
  versicolor       0.91      1.00      0.95        10
   virginica       1.00      0.90      0.95        10

    accuracy                           0.97        30
```

---

## 📝 License

This project is licensed under the MIT License.
