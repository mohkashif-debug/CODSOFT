# 🎬 Movie Genre Classification using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9-blue?logo=python">
  <img src="https://img.shields.io/badge/NLP-TF--IDF-orange">
  <img src="https://img.shields.io/badge/ML-Scikit--Learn-yellow?logo=scikitlearn">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey">
</p>

---

## 📌 Project Overview

The **Movie Genre Classification** project aims to automatically predict the genre of a movie based on its **plot summary** using Natural Language Processing (NLP) and Machine Learning techniques.

This system transforms textual data into numerical features and uses trained models to classify movies into genres such as:

* 🎭 Drama
* 😂 Comedy
* 🔪 Thriller
* ❤️ Romance
* 🚀 Sci-Fi

---

## 🎯 Objectives

* Convert text data into meaningful numerical representations
* Train ML models for genre classification
* Evaluate model performance using multiple metrics
* Build a scalable NLP-based classification pipeline

---

## 🖼️ Project Workflow

```id="wf92jd"
        ┌────────────────────┐
        │ Movie Dataset      │
        │ (Plots + Genres)   │
        └─────────┬──────────┘
                  ↓
        ┌────────────────────┐
        │ Text Preprocessing │
        │ Cleaning, Stopwords│
        └─────────┬──────────┘
                  ↓
        ┌────────────────────┐
        │ Feature Extraction │
        │ TF-IDF / Embedding │
        └─────────┬──────────┘
                  ↓
        ┌────────────────────┐
        │ Model Training     │
        │ NB | SVM | RF      │
        └─────────┬──────────┘
                  ↓
        ┌────────────────────┐
        │ Model Evaluation   │
        └─────────┬──────────┘
                  ↓
        ┌────────────────────┐
        │ Genre Prediction   │
        └────────────────────┘
```

---

## 🗂️ Dataset

* 📄 `kaggle_movie_train.csv`
* 📄 `kaggle_movie_test.csv`

### Key Columns:

* `plot` → Movie description
* `genre` → Target label

---

## ⚙️ Tech Stack

| Category       | Tools Used   |
| -------------- | ------------ |
| Programming    | Python 🐍    |
| NLP            | NLTK / spaCy |
| ML Library     | Scikit-learn |
| Feature Method | TF-IDF       |

---

## 🔍 Text Processing Steps

* Lowercasing text
* Removing special characters
* Removing stopwords
* Tokenization
* Vectorization using **TF-IDF**

---

## 🤖 Machine Learning Models

### 📊 Naive Bayes

* Fast and efficient for text classification
* Works well with TF-IDF features

### 📐 Support Vector Machine (SVM)

* Effective in high-dimensional text data
* Provides strong classification boundaries

### 🌳 Random Forest

* Handles non-linear relationships
* Ensemble-based approach

---

## 📊 Evaluation Metrics

* ✅ Accuracy
* 🎯 Precision
* 🔁 Recall
* 📈 F1-Score

---

## 📸 Visualizations (Sample)

<p align="center">
  <img src="https://via.placeholder.com/600x300?text=Confusion+Matrix">
</p>

<p align="center">
  <img src="https://via.placeholder.com/600x300?text=Model+Accuracy+Comparison">
</p>

---

## 🧠 Feature Engineering Example

```python id="z9x1hs"
from sklearn.feature_extraction.text import TfidfVectorizer

vectorizer = TfidfVectorizer(max_features=5000)
X = vectorizer.fit_transform(text_data)
```

---

## 🔮 Prediction Example

```python id="c2kpq7"
sample_plot = ["A young hero saves the world from alien invasion"]
prediction = model.predict(vectorizer.transform(sample_plot))
print(prediction)
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone Repository

```bash id="clp91d"
git clone https://github.com/your-username/movie-genre-classification.git
cd movie-genre-classification
```

### 2️⃣ Install Dependencies

```bash id="g92kds"
pip install pandas scikit-learn nltk
```

### 3️⃣ Run Notebook / Script

```bash id="plm28x"
jupyter notebook
```

---

## ⚠️ Challenges Faced

* Handling unstructured text data
* Feature selection for NLP
* Multi-class classification complexity

---

## 🚀 Future Improvements

* 🔥 Use Deep Learning (LSTM / BERT)
* 🌐 Deploy using Streamlit
* 📊 Add real-time predictions
* 🧠 Use word embeddings (Word2Vec, GloVe)

---

## 🏆 Key Learnings

* Natural Language Processing pipeline
* Feature extraction techniques
* Multi-class classification
* Model evaluation strategies

---

## 📜 License

This project is licensed under the **MIT License**

---

## 🤝 Contributions

Contributions are welcome! Feel free to fork and improve.

---

## 👨‍💻 Author

**Mohammad Kashif**
Final Year CSE Student

---

## ⭐ Support

If you found this project useful, give it a ⭐ on GitHub!

---
