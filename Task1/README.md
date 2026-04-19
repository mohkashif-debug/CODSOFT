# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using various machine learning algorithms. The goal is to classify transactions as **fraudulent (1)** or **legitimate (0)** based on transaction data.

The system trains multiple models and compares their performance using evaluation metrics like accuracy, confusion matrix, and classification report.

---

## 🚀 Features

* Data preprocessing and splitting
* Multiple ML models implementation:

  * Random Forest
  * Logistic Regression
  * Support Vector Machine (SVM)
  * K-Nearest Neighbors (KNN)
* Model evaluation using:

  * Accuracy Score
  * Confusion Matrix
  * Classification Report
* User input-based fraud prediction

---

## 🗂️ Dataset

* File used: `cdd.csv`
* Contains transaction details with a target column:

  * **Class = 0 → Legitimate**
  * **Class = 1 → Fraud**

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas
* Scikit-learn

---

## 📊 Machine Learning Models Used

### 1. Random Forest

* Ensemble learning method
* Handles imbalance and complex patterns well

### 2. Logistic Regression

* Simple and interpretable model
* Good baseline performance

### 3. Support Vector Machine (SVM)

* Effective in high-dimensional spaces

### 4. K-Nearest Neighbors (KNN)

* Instance-based learning algorithm

---

## 🔄 Workflow

1. Load dataset
2. Split into features (X) and target (y)
3. Train-test split (80% training, 20% testing)
4. Train models
5. Evaluate models
6. Predict fraud based on user input

---

## 📈 Evaluation Metrics

* Accuracy Score
* Confusion Matrix
* Precision, Recall, F1-score (Classification Report)

---

## 🧠 Model Training

```python
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(random_state=42)
model.fit(X_train, y_train)
```

---

## 🔮 Prediction

The system allows users to input feature values manually and predicts whether the transaction is fraudulent.

```python
predicted_class = model.predict([user_input])
```

---

## ▶️ How to Run

1. Install required libraries:

```bash
pip install pandas scikit-learn
```

2. Place dataset file `cdd.csv` in the project directory

3. Run the Python script:

```bash
python python.py
```

4. Enter feature values when prompted

---

## 📌 Output

* Model performance comparison
* Fraud prediction result

---

## ⚠️ Note

* Dataset imbalance may affect accuracy
* Consider using techniques like SMOTE or undersampling for better performance

---

## 📚 Future Improvements

* Use Deep Learning models
* Apply feature engineering
* Handle class imbalance more effectively
* Deploy as a web app

---

## 👨‍💻 Author

* Developed as a Machine Learning project for academic purposes

---

## ⭐ Conclusion

This project demonstrates how machine learning can be applied to detect fraudulent transactions effectively by comparing multiple models and selecting the best-performing one.

---
