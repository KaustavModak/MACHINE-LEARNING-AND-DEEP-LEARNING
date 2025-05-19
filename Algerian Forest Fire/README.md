# Algerian Forest Fires Prediction System

This repository contains both data analysis workflows and a web application for predicting Forest Fire Weather Index (FWI) using meteorological and environmental data. The project focuses on forest fire incidents in Algeria, specifically in the **Bejaia** and **Sidi-Bel Abbes** regions during the summer season of 2012.

---

## 📂 Repository Contents

| File Name                                | Description |
|------------------------------------------|-------------|
| `Algerian_forest_fires_dataset.csv`      | The original dataset from the UCI Machine Learning Repository. |
| `Algerian_forest_fires_cleaned_dataset.csv` | A cleaned and preprocessed version of the original dataset. |
| `code1.ipynb`                             | Jupyter Notebook for data exploration, cleaning, and visualization. |
| `code2.ipynb`                             | Jupyter Notebook for machine learning model building and evaluation. |
| `application.py`                          | Flask web application for FWI prediction. |
| `models/ridge.pkl`                        | Serialized Ridge Regression model for predictions. |
| `models/scaler.pkl`                       | Serialized StandardScaler for feature normalization. |
| `templates/welcome.html`                  | Welcome page template for the web application. |
| `templates/home.html`                     | Input form and prediction result display template. |

---

## 📊 Dataset Description

The dataset includes 244 instances and 12 attributes (meteorological and FWI components), collected daily. It is segmented into two classes:
- **Fire**: days when a fire occurred
- **Not Fire**: days without fire

### Key Attributes:
- **Temperature (°C)**, **Relative Humidity (%)**, **Wind Speed (km/h)**, **Rain (mm)**
- **FWI Components**: FFMC, DMC, DC, ISI, BUI, FWI
- **Date**, **Region**, and **Target class** (Fire/Not Fire)

---

## 🧪 Project Workflow

### 1. Data Exploration & Cleaning (`code1.ipynb`):
- Load and inspect the raw dataset.
- Handle missing or erroneous data entries.
- Convert data types, encode categorical features, and normalize numerical features.
- Visualize correlations between meteorological parameters and fire occurrences.

### 2. Machine Learning Model (`code2.ipynb`):
- Feature selection and engineering.
- Train/test split.
- Classification models applied: Logistic Regression, Decision Trees, Random Forest, SVM.
- Ridge Regression model trained for FWI prediction.
- Model performance evaluation using appropriate metrics.

### 3. Web Application (`application.py`):
- Flask-based web interface for prediction deployment.
- User input for meteorological parameters.
- Real-time FWI prediction using the trained Ridge Regression model.

---

## 🚀 Running the Web Application

1. Ensure all requirements are installed:
```bash
pip install flask pandas numpy scikit-learn
```

2. Run the Flask application:
```bash
python application.py
```

3. Navigate to `http://localhost:5000/` in your web browser.
4. Use the welcome page or go to `/predictdata` to access the prediction form.
5. Enter the required parameters and submit to get FWI predictions.

### Input Parameters:
- Temperature (°C)
- RH (Relative Humidity %)
- Ws (Wind Speed km/h)
- Rain (mm)
- FFMC (Fine Fuel Moisture Code)
- DMC (Duff Moisture Code)
- ISI (Initial Spread Index)
- Classes (Fire/Not Fire classification)
- Region (Bejaia/Sidi-Bel Abbes)

---

## 🎯 Objectives

- Identify significant environmental factors influencing forest fires.
- Build predictive models for early detection of fire risks.
- Provide an easy-to-use interface for forest fire risk assessment.
- Demonstrate a complete data science workflow from analysis to deployment.

---

## 📚 Data Source

The data is publicly available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Algerian+Forest+Fires+Dataset).

---

## 📄 License

This project is distributed under the MIT License. Use freely with attribution.

---

## 👨‍💻 Author

Developed as part of a forest fire risk analysis and prediction system for educational and research purposes.
