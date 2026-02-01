# 🐦 Twitter Sentiment Analysis: ML Model Comparison

## 📌 Project Overview
Sentiment analysis is a key tool in understanding public opinion. This project implements a Natural Language Processing (NLP) pipeline to classify tweets as Positive or Negative. I compared three different Machine Learning algorithms to find the most effective model for this large-scale dataset (Sentiment140).

## ⚙️ Technical Workflow
1. **Data Acquisition:** Used `kagglehub` to programmatically download the Sentiment140 dataset.
2. **Pre-processing:** * Filtered polarities and mapped labels (0 = Negative, 1 = Positive).
   * Text cleaning (Lowercasing).
   * Split data (80% Train / 20% Test) to ensure unbiased evaluation.
3. **Feature Engineering:** Implemented **TF-IDF Vectorization** with an `ngram_range=(1,2)` to capture both single words and common phrases.
4. **Model Training & Comparison:**
   * **Bernoulli Naive Bayes:** Ideal for discrete data.
   * **Linear SVC (SVM):** Effective for high-dimensional text data.
   * **Logistic Regression:** A robust baseline for binary classification.



## 📊 Results & Performance
The models were evaluated based on **Accuracy**, **Precision**, and **Recall**. 
* **Logistic Regression** and **SVM** typically show high performance in such text-heavy tasks.
* **BernoulliNB** provides a fast and efficient alternative for binary text features.

## 🛠️ Tools & Libraries
* **Python:** 3.11
* **Environment:** Google Colab
* **ML Libraries:** Scikit-Learn (TF-IDF, BernoulliNB, LinearSVC, LogisticRegression)
* **Data Management:** Pandas, Zipfile, OS

---
*This project serves as a core part of my Data Science portfolio as I pursue an internship in **Data Analysis**.*# Twitter-Sentiment-Analysis-ML
