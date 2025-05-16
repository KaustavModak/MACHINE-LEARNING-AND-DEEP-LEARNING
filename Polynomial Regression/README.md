
# Polynomial Regression in Python

This project demonstrates how to perform **Polynomial Regression** using Python and popular libraries like NumPy, Matplotlib, and Scikit-Learn. The goal is to show how polynomial features can be used to model non-linear data using linear models.

## 📁 File Structure

- `poly_reg.ipynb`: A Jupyter notebook implementing polynomial regression, from data creation to model training and visualization.
- `README.md`: This file.

## 📌 Features

- **Data Generation or Loading**: Creates synthetic datasets or can be modified to load real-world datasets.
- **Data Preprocessing**: Normalization and polynomial feature transformation.
- **Model Training**:
  - Linear Regression (baseline)
  - Polynomial Regression using `PolynomialFeatures` from Scikit-Learn
- **Model Evaluation**:
  - Comparison of linear vs. polynomial fit
  - Metrics like Mean Squared Error (MSE) and R² Score
- **Visualization**:
  - Scatter plots of data
  - Regression curves for different polynomial degrees
  - Error metrics visualization (if included)

## 🔧 Requirements

Make sure you have the following Python packages installed:

```bash
pip install numpy matplotlib scikit-learn
```

## ▶️ How to Run

1. Download the repository or just the notebook file.
2. Launch Jupyter Notebook:

```bash
jupyter notebook poly_reg.ipynb
```

3. Execute all cells to view results and visualizations.

## 💡 Use Cases

- Understanding polynomial regression intuitively.
- Comparing linear and non-linear regression models.
- Practicing machine learning model evaluation and tuning.
- Using polynomial transformations to model curved trends in data.

## 📚 References

- [Scikit-Learn Polynomial Features](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.PolynomialFeatures.html)
- [Scikit-Learn Linear Models](https://scikit-learn.org/stable/modules/linear_model.html)
- [Jupyter Documentation](https://jupyter.org/)
