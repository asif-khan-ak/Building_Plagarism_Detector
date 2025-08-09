# 📚 Plagiarism Detection Web App using Machine Learning & Flask

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Flask](https://img.shields.io/badge/Flask-Web--Framework-black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![NLP](https://img.shields.io/badge/NLP-TF--IDF-yellowgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

This project is a complete **Plagiarism Detection System** that combines **Natural Language Processing** with **Machine Learning** and a **Flask-powered Web Interface**. Users can input text directly on the web app, and the model will detect whether plagiarism is likely based on pre-trained models.

---

## 📁 Dataset Preparation

- The custom dataset contains text-based pairs of documents labeled as plagiarized or not plagarised.
- Preprocessed and cleaned for model input.

---

## 🧠 Machine Learning Overview

The following classification models were trained and evaluated:

- ✅ **Random Forest** *(Best performance)*
- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVM)

### 📊 Features Used

- **TF-IDF Vectorization** of input text
- Cosine similarity
- Text pre-processing (tokenization, stopword removal, lowercasing)

The **Random Forest classifier** achieved the highest accuracy (~95%) and was selected for deployment.

---

## 🌐 Flask Web Application

The project includes a responsive, minimal front-end using HTML/CSS. It allows users to:

- Paste custom text input
- Click to run detection
- View real-time results (Plagiarism Detected / No Plagiarism Detected)

### 📁 Key Files

| File                    | Description                                      |
|-------------------------|--------------------------------------------------|
| `app.py`                | Flask backend connecting model to UI             |
| `index.html`            | Frontend HTML template for text input            |
| `model.pkl`             | Pickled Random Forest model                      |
| `ztfidf_vectorizer.pkl` | Pickled TF-IDF vectorizer                        |

---

## 🧰 Technologies Used

- **Python** (3.8+)
- **scikit-learn** – TF-IDF Vectorizer, cosine similarity
- **Pickle**
- **Flask**

---
