# Logistic Regression from Scratch in Python

This repository contains a detailed implementation of **Logistic Regression** from scratch using only NumPy. The aim is to understand the fundamental mechanics of binary classification without relying on high-level libraries like `scikit-learn`.

## 📌 What is Logistic Regression?

Logistic Regression is a **supervised learning** algorithm used for **binary classification** problems. It estimates the probability that a given input belongs to a particular category.

### 🔢 Mathematical Background

- **Hypothesis Function**:  
  \( h_\theta(x) = \frac{1}{1 + e^{-\theta^T x}} \)

- **Cost Function** (Log Loss):  
  \( J(\theta) = -\frac{1}{m} \sum_{i=1}^{m} [y^{(i)} \log(h_\theta(x^{(i)})) + (1 - y^{(i)}) \log(1 - h_\theta(x^{(i)}))] \)

- **Optimization**:  
  Gradient Descent is used to minimize the cost function.

---

## 📁 Project Structure

```
.
├── Logistic Regression Implementation.ipynb
└── README.md
```

- `Logistic Regression Implementation.ipynb`: Contains the complete step-by-step implementation including:
  - Data simulation or import
  - Model logic (sigmoid, cost, gradient descent)
  - Evaluation metrics
  - Visualization (if included)

---

## ⚙️ Features

- ✅ Implements Logistic Regression using **NumPy only**
- ✅ Includes a **vectorized** approach for better performance
- ✅ Implements **gradient descent** optimization
- ✅ Displays **loss during training**
- ✅ Predicts and evaluates on test data
- ✅ Accuracy calculation and comparison

---

## 🛠️ How to Run

### 📦 Prerequisites

- Python 3.x
- Jupyter Notebook
- NumPy
- (Optional) Matplotlib

Install required packages via pip:

```bash
pip install numpy matplotlib notebook
```

### 🚀 Run Instructions

```bash
jupyter notebook
```

Then open the notebook file and execute each cell in order.

---

## 📊 Outputs

- Final trained weights
- Decision boundary (if visualization is implemented)
- Accuracy score
- Loss convergence plot over iterations

---

## ✅ Use Cases

- Understanding the fundamentals of binary classification
- Educational purposes for learning machine learning
- Benchmarking with `scikit-learn`
- Custom model extensions

---

## 🔮 Possible Improvements

- Add **L2 regularization**
- Extend to **multiclass classification** using One-vs-Rest
- Compare with `sklearn.LogisticRegression`
- Add **ROC-AUC**, **Precision**, **Recall** metrics

---

## 📄 License

This project is licensed under the MIT License. You are free to use, modify, and distribute this work.

---

## 👨‍💻 Author

Created by [Your Name]  
Feel free to connect via GitHub or LinkedIn!
