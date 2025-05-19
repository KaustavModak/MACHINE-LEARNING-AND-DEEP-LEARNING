
# Algerian Forest Fires Analysis Project

This repository contains a complete workflow for analyzing forest fire incidents in Algeria using real-world meteorological and environmental data. The analysis is focused on data collected in two regions: **Bejaia** and **Sidi-Bel Abbes** during the summer season of 2012.

---

## 📂 Repository Contents

| File Name                                | Description |
|------------------------------------------|-------------|
| `Algerian_forest_fires_dataset.csv`      | The original dataset from the UCI Machine Learning Repository. |
| `Algerian_forest_fires_cleaned_dataset.csv` | A cleaned and preprocessed version of the original dataset. |
| `code1.ipynb`                             | Jupyter Notebook for data exploration, cleaning, and visualization. |
| `code2.ipynb`                             | Jupyter Notebook for machine learning model building and evaluation. |

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
- Model performance evaluated using accuracy, precision, recall, and confusion matrix.

---

## 🛠️ Installation & Requirements

Ensure Python 3.7+ is installed. Install required libraries with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

You can run the notebooks using Jupyter or any compatible environment like VSCode or Google Colab.

---

## 🎯 Objectives

- Identify significant environmental factors influencing forest fires.
- Build predictive models for early detection of fire risks.
- Demonstrate data science workflows from raw data to predictive analytics.

---

## 📚 Data Source

The data is publicly available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Algerian+Forest+Fires+Dataset).

---

## 📄 License

This project is distributed under the MIT License. Use freely with attribution.

---

## 👨‍💻 Author

Developed as part of a forest fire risk analysis project for educational and research purposes.
