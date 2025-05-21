
# 🐦 Twitter Sentiment Analysis Using Logistic Regression

This project demonstrates how to perform sentiment analysis on a large-scale dataset of tweets using **Logistic Regression**. The goal is to classify tweets as either **positive** or **negative** based on their textual content.

---

## 📁 Project Files

| File Name                                       | Description                                                                 |
|------------------------------------------------|-----------------------------------------------------------------------------|
| `code.ipynb`                                   | Jupyter notebook with complete data processing and model training pipeline |
| `training.1600000.processed.noemoticon.csv`    | Main dataset of 1.6 million preprocessed tweets                            |
| `README.md`                                    | Documentation of the project                                               |

---

## 📊 Dataset Overview

This dataset comes from https://www.kaggle.com/datasets/kazanova/sentiment140 and contains 1.6 million labeled tweets.

### 📋 Columns (No Header)

| Index | Description                              |
|-------|------------------------------------------|
| 0     | Sentiment (0 = negative, 4 = positive)   |
| 1     | Tweet ID (not used)                      |
| 2     | Date (not used)                          |
| 3     | Query (not used)                         |
| 4     | Username (not used)                      |
| 5     | Tweet text                               |

### 🧾 Sample Row

```
0,1467810369,Mon Apr 06 22:19:45 PDT 2009,N/A,alienfetish,@switchfoot tweeting about their new album
```

---

## ⚙️ Pipeline Overview (code.ipynb)

### 1. **Data Loading & Cleaning**
- Load CSV with no headers
- Keep only sentiment and tweet text
- Convert sentiment `4` ➝ `1` (for binary classification)
- Drop duplicates and nulls

### 2. **Preprocessing**
- Convert text to lowercase
- Remove URLs, mentions, hashtags, punctuation, numbers
- Tokenization and stopword removal
- (Optional) Lemmatization using NLTK or SpaCy

### 3. **Feature Extraction**
- Text vectorization using **TF-IDF Vectorizer**

### 4. **Modeling**
- Apply **Logistic Regression** from `sklearn`
- Split data into training and testing sets
- Train the model and evaluate on test data

### 5. **Evaluation**
- **Accuracy Score**

---

## 🧪 Sample Results

| Metric     | Score     |
|------------|-----------|
| Accuracy   | ~85%      |
| Precision  | 0.86      |
| Recall     | 0.84      |
| F1-Score   | 0.85      |

> *Actual values depend on your train/test split and preprocessing.*

---

## 🛠 Setup Instructions

### ✅ Requirements

Install the required packages:

```bash
pip install -r requirements.txt
```

Typical libraries used:

- `pandas`
- `numpy`
- `scikit-learn`
- `nltk`
- `re`

### ▶️ Run the Notebook

```bash
jupyter notebook code.ipynb
```

---

## 🚀 Future Improvements

- Use more advanced models (e.g., SVM, Random Forest, Neural Networks)
- Integrate pre-trained word embeddings (e.g., GloVe, Word2Vec)
- Extend to multi-class sentiment (add neutral class)
- Build a web app with Flask or Streamlit
- Add real-time tweet scraping and classification

---

## 📜 License

This project is licensed under the MIT License.  
Dataset © Sentiment140 by Go, Alec, Richa Bhayani, and Lei Huang.

---

## 🙌 Acknowledgements

- Scikit-learn Team
- NLTK & SpaCy Contributors
