# 🚀 Scalable Sentiment Analysis on Twitter Data Using Apache Spark

A scalable sentiment analysis system that processes large-scale Twitter data using **Apache Spark (PySpark)** and **Machine Learning**. The project uses **TF-IDF** for text feature extraction and **Random Forest** for binary sentiment classification.

---

## 📌 Overview

Social media platforms generate enormous amounts of textual data every day. Analyzing this data manually is difficult because of its size and unstructured nature.

This project develops a scalable sentiment analysis pipeline capable of processing a large Twitter dataset and classifying tweets into:

- 🟢 Positive
- 🔴 Negative

The system combines Natural Language Processing (NLP), distributed data processing, and machine learning using Apache Spark.

---

## 🎯 Objectives

- Process a large-scale Twitter dataset efficiently.
- Perform text preprocessing using PySpark.
- Convert textual data into numerical features using **TF-IDF**.
- Train a **Random Forest classifier** for sentiment prediction.
- Evaluate the model using standard classification metrics.
- Provide an interactive sentiment analyzer for new text inputs.

---

## 🗂️ Dataset

### Sentiment140

The project uses the **Sentiment140 dataset**, containing approximately **1.6 million tweets** labeled with positive or negative sentiment.

**Dataset characteristics:**

| Property | Description |
|---|---|
| Dataset | Sentiment140 |
| Approx. Records | 1.6 Million Tweets |
| Task | Binary Sentiment Classification |
| Classes | Positive / Negative |
| Data Type | Twitter Text |

The dataset was originally introduced by Go, Bhayani, and Huang for large-scale Twitter sentiment classification.

---


# 📊 Dataset

## Sentiment140

The project uses the **Sentiment140** dataset.
Dataset characteristics:

- Approximately **1.6 million tweets**
- Binary sentiment classification
- Positive and negative sentiment classes
- Text-based social media data
- Suitable for large-scale sentiment analysis

### Dataset Format

The original dataset contains fields such as:


---

# 🛠️ Technologies Used

## Big Data

- Apache Spark
- PySpark
- Spark MLlib

## Programming

- Python

## Machine Learning

- Random Forest
- TF-IDF
- Binary Classification

## Natural Language Processing

- Text Cleaning
- Tokenization
- Stopword Removal
- Feature Extraction

## Development Environment

- Google Colab
- Google Drive

## Dataset

- Sentiment140

---


---

# ⚡ Why Apache Spark?

Processing 1.6 million tweets involves a large amount of textual data.
Apache Spark is suitable for this task because it provides:

- Distributed data processing
- In-memory computation
- Scalable machine learning
- DataFrame-based processing
- Integration with MLlib
- Efficient processing of large datasets

Instead of treating the dataset as a small collection of records, Spark provides a framework for processing large-scale data efficiently.

---

# 🌳 Why Random Forest?

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees.
For sentiment classification, it can learn patterns from the numerical TF-IDF representation of tweets.
Advantages include:

- Handles high-dimensional feature spaces
- Ensemble-based learning
- Can model nonlinear relationships
- Provides robust classification performance
- Available through Spark MLlib

---

# 🔢 TF-IDF

TF-IDF stands for:
**Term Frequency – Inverse Document Frequency**
It assigns importance to words based on how frequently they occur in a document and how common they are across documents.

### TF

Term Frequency measures how frequently a word occurs in a document.

### IDF

Inverse Document Frequency reduces the importance of words that appear in many documents.

### TF-IDF

The combination gives a numerical representation of the importance of words.
Conceptually:



This converts text into numerical features that can be used by the machine learning model.

---

# 📈 Model Evaluation

The trained model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Final Model Results

| MetricScore |            |
| ----------- | ---------- |
| Accuracy    | **66.52%** |
| Precision   | **62.54%** |
| Recall      | **82.60%** |
| F1-Score    | **71.18%** |

These results are based on the project's final reported evaluation.

---

# 🧮 Confusion Matrix

The model produced the following confusion matrix:

| Actual / PredictedNegativePositive |        |         |
| ---------------------------------- | ------ | ------- |
| Negative                           | 80,455 | 79,120  |
| Positive                           | 27,832 | 132,086 |

## 🏗️ System Architecture

```text
                 ┌──────────────────────┐
                 │    Sentiment140      │
                 │    1.6M Tweets       │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │     Data Loading     │
                 │      PySpark         │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │  Text Preprocessing  │
                 │ Cleaning & Tokenizing│
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │   Stopword Removal   │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │      HashingTF       │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │        IDF           │
                 │       TF-IDF         │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │   Random Forest      │
                 │     Classifier       │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │ Sentiment Prediction │
                 └──────────┬───────────┘
                            │
                    ┌───────┴────────┐
                    ▼                ▼
               🟢 Positive       🔴 Negative
---


## 📚 References
Go, A., Bhayani, R., & Huang, L. (2009).
Twitter Sentiment Classification using Distant Supervision.
Stanford University.
Breiman, L. (2001).
Random Forests.
Machine Learning, 45, 5–32.
Apache Spark Documentation.
Spark MLlib – Machine Learning Library.
Sentiment140 Dataset.
A large-scale dataset for sentiment analysis of Twitter data.

----

## 👥 Team Members
MITHRAVINDA U
MUHAMMED NASIF CP
MAYUG B
MIDHUNA
JISTO JOSE
JOEL MATHEW SAJI
----
