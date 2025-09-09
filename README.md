# 🛒 Shopee Sentiment Analysis – Naïve Bayes  

This repository contains a sentiment analysis project on **Shopee app reviews** collected from Google Play Store.  
The project applies **Naïve Bayes classifier** with **TF-IDF feature extraction** to classify reviews into **positive** and **negative** sentiments.  

---

## 📊 Dataset  
- **Source**: Scraped from Google Play Store  
- **Total Reviews**: 796  
- **Features**:  
  - `reviewId` → unique identifier  
  - `username` → reviewer name  
  - `content` → review text  
  - `score` → user rating (1–5)  
  - Other metadata (date, appVersion, replies, etc.)  

### Labeling  
- **Negative** → score 1–2  
- **Positive** → score 3–5  

---

## 🔎 Methodology  
1. **Data Collection** → Web scraping from Google Play Store.  
2. **Preprocessing** → text cleaning, lowercasing, stopword removal, tokenization, stemming.  
3. **Feature Extraction** → TF-IDF weighting.  
4. **Classification** → Naïve Bayes model applied on training data.  
5. **Evaluation** → Accuracy, Precision, Recall, F1-Score via Confusion Matrix.  

---

## 🛠️ Tools & Libraries  
- Python  
- Pandas, Numpy  
- Scikit-learn (TF-IDF, Naïve Bayes, metrics)  
- Matplotlib / Seaborn (visualization)  

---

## 📈 Results  
- **Accuracy**: 81%  
- **Precision (Positive)**: 85%  
- **Recall (Positive)**: 63%  
- **F1-Score (Positive)**: 0.72  

Confusion Matrix:  
- True Positive (76), True Negative (33)  
- False Positive (7), False Negative (19) 
