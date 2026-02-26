# 🧠 Job Title Prediction using NLP

This project builds a Natural Language Processing (NLP) model to predict job titles based on job description text.

The problem is formulated as a supervised multi-class classification task using machine learning techniques.

---

## 📌 Problem Statement

Given a job description, the goal is to predict the corresponding job title.

This helps automate resume screening, job classification, and recruitment analytics.

---

## 🛠 Project Workflow

### 1️⃣ Text Preprocessing
- Lowercasing
- Removing special characters
- Tokenization
- Stopword removal
- Lemmatization

### 2️⃣ Feature Engineering
- TF-IDF Vectorization
- Word Embeddings (Word2Vec)
- Sequence Tokenization (for LSTM)

### 3️⃣ Models Implemented
- Multinomial Naive Bayes
- Logistic Regression
- Word2Vec + Logistic Regression
- LSTM
- Transformer-based modeling (BERT)

---

## 📊 Model Selection

After comparing multiple modeling approaches:

- Classical ML models performed strong for structured job description data.
- Logistic Regression with TF-IDF features provided stable and interpretable performance.
- Deep learning and transformer models were explored for performance comparison and architectural understanding.

The final selected approach balances performance, interpretability, and computational efficiency.

---

## 📂 Repository Structure

- `NLP_Project.ipynb` — Complete modeling workflow  


---

## 🧠 Key Highlights

- End-to-end NLP pipeline
- Multi-model comparison
- Feature engineering experiments
- Deep learning implementation
- Transformer exploration
- Real-world text classification use case

---

## 🚀 Skills Demonstrated

- Natural Language Processing  
- Text Preprocessing  
- Feature Engineering  
- Machine Learning  
- Deep Learning (LSTM)  
- Transformer-based Modeling  
- Model Evaluation & Selection  
