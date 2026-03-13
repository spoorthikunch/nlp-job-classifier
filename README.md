# 🔍 NLP Job Title Classification

End-to-end NLP pipeline to classify job titles from job description text.
Benchmarked 4 modeling approaches — **TF-IDF + Logistic Regression achieved 83% accuracy**, outperforming fine-tuned BERT.

## 📊 Model Comparison Results

| Model | Accuracy |
|---|---|
| TF-IDF + Logistic Regression ✅ | **~83%** (best) |
| BERT (bert-base-uncased fine-tuned) | ~79% |
| TF-IDF + Naive Bayes | ~75% |
| Word2Vec + Logistic Regression | moderate |
| LSTM | did not outperform TF-IDF baseline |

## 🎯 Key Insight

**TF-IDF + Logistic Regression outperformed fine-tuned BERT.**

Why? The dataset is strongly keyword-driven — job descriptions 
contain highly discriminative words like "Python", "Java", "nurse", 
"accountant" that directly signal the job title. With limited 
training data, simpler models generalise better than complex 
deep learning architectures.

> **Model selection must be driven by data characteristics — not model complexity.**

## 🛠 Tech Stack
Python • Scikit-learn • HuggingFace Transformers • PyTorch • 
TF-IDF • Word2Vec • LSTM • BERT • NLTK • Streamlit

## 🔄 Project Workflow

**Text Preprocessing:**
- Lowercase, remove special characters
- Tokenization and stopword removal
- Lemmatization using WordNet

**Modeling Approaches:**
- TF-IDF + Naive Bayes (baseline)
- TF-IDF + Logistic Regression
- Word2Vec + Logistic Regression
- LSTM with embedding layers
- Fine-tuned BERT (bert-base-uncased, 2 epochs, lr 2e-5)

**Evaluation Metrics:**
- Accuracy, Precision, Recall, F1-score
- Confusion matrix analysis

## 🚀 Run Locally
```bash
git clone https://github.com/spoorthikunch/nlp-job-classifier.git
cd nlp-job-classifier
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
streamlit run app.py
```

## 📁 Repository Structure
- `NLP_Project.ipynb` — Complete modeling workflow
- `app.py` — Streamlit deployment
- `requirements.txt` — Dependencies

## 👩‍💻 Author
Spoorthi G Kunch
[LinkedIn](https://www.linkedin.com/in/spoorthi-kunch-5a0464286) | 
[GitHub](https://github.com/spoorthikunch)
