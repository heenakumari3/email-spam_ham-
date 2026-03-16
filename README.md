# Email Spam Detection (Spam vs Ham)

## Project Overview
Email spam detection is an important task in natural language processing (NLP). Spam emails can contain advertisements, phishing attempts, or malicious links that may harm users.

This project builds a machine learning model to automatically classify emails or messages as **Spam** or **Ham (Not Spam)** using text processing techniques and machine learning algorithms.

---

## Problem Statement
With the increasing use of email communication, spam messages have become a major problem. The goal of this project is to build a model that can **identify spam emails and filter them automatically**.

The model learns patterns from labeled email messages and predicts whether a new message is spam or ham.

---

## Dataset
The dataset contains email or SMS messages labeled as either **spam** or **ham**.

Typical columns in the dataset include:

- **label** – Spam or Ham
- **message** – Text content of the email or SMS

Target variable:
- **Spam** → Unwanted or promotional message  
- **Ham** → Legitimate message

---

## Project Workflow

### 1. Data Loading
The dataset is loaded using **Pandas** and inspected to understand its structure.

### 2. Data Preprocessing
Text data is cleaned and prepared for machine learning:

- Lowercasing text
- Removing punctuation
- Removing stopwords
- Tokenization

### 3. Text Vectorization
Text data cannot be directly used by machine learning models, so it is converted into numerical form using:

**TF-IDF (Term Frequency – Inverse Document Frequency)**

---

### 4. Model Building
Two machine learning models were used for classification:

**1. Naive Bayes**

Naive Bayes is a probabilistic classifier commonly used for text classification tasks like spam detection.

**2. Support Vector Machine (SVM)**

SVM is a powerful classification algorithm that finds the best boundary to separate spam and ham messages.

---

### 5. Model Evaluation
The models were evaluated using:

- Accuracy
- Precision
- Recall
- Confusion Matrix

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TF-IDF Vectorizer
- Natural Language Processing (NLP)

---

## Project Structure

```
email-spam-detection
│
├── README.md
├── spam_ham(1).ipynb
└── spam_ham_dataset.csv
```

---

## Key Insights
- Text vectorization is essential for converting messages into machine learning features.
- Naive Bayes performs well for basic text classification tasks.
- SVM provides strong classification performance for spam detection problems.

---

## Business Impact
Spam detection systems help:

- Filter unwanted emails automatically
- Protect users from phishing attacks
- Improve email service quality
- Enhance cybersecurity in communication systems

---

## Future Improvements
- Use deep learning models such as LSTM or BERT
- Perform hyperparameter tuning
- Deploy the model as an email spam filtering application
- Implement real-time spam detection

---
