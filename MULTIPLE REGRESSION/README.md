# 📊 Economic Index Prediction using Multiple Linear Regression

This project demonstrates the application of **Multiple Linear Regression (MLR)** to predict an **Economic Index** based on various economic indicators. The dataset used is `economic_index.csv`, and the analysis is implemented in the Jupyter Notebook `multiple_lr.ipynb`.

---

## 🧠 Objective

The primary goal of this project is to:

- Explore relationships between economic indicators.
- Build a predictive model for the economic index.
- Interpret the influence of each feature on the target variable.
- Evaluate model performance and suggest improvements.

---

## 📁 Project Structure

```
project-folder/
│
├── economic_index.csv        # Dataset with multiple economic variables
├── multiple_lr.ipynb         # Jupyter Notebook with MLR implementation
└── README.md                 # This documentation file
```

---

## 📦 Dependencies

This project uses Python 3 and the following libraries:

- `pandas` – for data handling
- `numpy` – for numerical operations
- `matplotlib` / `seaborn` – for data visualization
- `scikit-learn` – for model training and evaluation

Install them using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```



## 📄 Dataset Overview

The dataset `economic_index.csv` contains multiple columns:

- **Independent variables (features)**: Economic indicators such as inflation rate, GDP growth, unemployment rate, etc.
- **Dependent variable (target)**: An aggregated **Economic Index** measuring economic performance.

The dataset is used to train and test a Multiple Linear Regression model.

---

## 🔍 Methodology

The notebook follows these major steps:

1. **Data Loading** – Read the CSV file using `pandas`.
2. **Data Cleaning** – Handle missing values and format data types if required.
3. **Exploratory Data Analysis (EDA)** – Visualize relationships using pairplots, heatmaps, and histograms.
4. **Correlation Matrix** – Identify multicollinearity.
5. **Model Training** – Use `LinearRegression()` from `sklearn.linear_model`.
6. **Prediction** – Predict economic index values from the input features.
7. **Model Evaluation**:
   - Coefficients and intercept
   - R² Score
   - RMSE / MAE (optional)
   - Residual Analysis

---

## 📈 Results & Insights

- The model outputs a regression equation showing how each variable contributes to the prediction.
- **R² score** provides the proportion of variance in the economic index explained by the features.
- Visualization of residuals helps assess model assumptions (e.g., homoscedasticity).
- Observations from EDA and coefficient analysis may offer policy insights.

---

## ⚠️ Limitations & Future Work

- **Multicollinearity** may affect coefficient interpretation.
- Feature engineering or variable transformation could improve model accuracy.
- Other models (e.g., Ridge, Lasso, or Tree-based regressors) may offer better generalization.

---

## 🧪 How to Use

1. Clone or download this repository.
2. Launch Jupyter Notebook in the project directory.
3. Open `multiple_lr.ipynb`.
4. Run each cell step-by-step and observe outputs.
5. Modify the dataset or model parameters to experiment.

---

## 📜 License

This project is open-source and free to use under the [MIT License](LICENSE).
