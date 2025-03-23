# Sentiment Analysis - Dicoding Data Science (Advanced Level)

## Overview
This project is an Advanced Data Science approach for Sentiment Analysis. Sentiment analysis is a subfield of Text Classification that aims to identify and evaluate opinions, attitudes, or emotions expressed in textual data. In this project, I analyzed user reviews of the game "Clash of Clans" to determine whether the sentiment is negative, positive, or neutral.

## Objective
**1. Data Scraping**
- Extracted 25,000 reviews from Google Play.
- Filtered reviews based on English language and Indonesia region.

**2. Data Preprocessing**
- Data Gathering: Collected raw data from the source.
- Data Assessment: Checked for missing values and inconsistencies.
- Data Cleaning: Removed unnecessary characters, stopwords, and handled missing values.

**3. Feature Extraction & Data Labeling**
- Feature Extraction:
   - TF-IDF (Term Frequency-Inverse Document Frequency)
   - Word2Vec (Word Embeddings)

- Data Labeling:
   - TextBlob (Polarity-based sentiment labeling)
   - VADER (Valence Aware Dictionary and sEntiment Reasoner)

**4. Using 3 schemas for training and testing**
- TF-IDF feature extraction, 80/20 data split, TextBlob labeling
- Word2Vec feature extraction, 80/20 data split, VADER labeling
- TF-IDF feature extraction, 70/30 data split, TextBlob labeling

## **Result:**
1. TF-IDF feature extraction, 80/20 data split, TextBlob labeling
   - Support Vector Machine(SVM)
     ```
     Support Vector Machine - accuracy_train: 0.98675
     Support Vector Machine - accuracy_test: 0.8772
     ```
   - Logistic Regression
     ```
     Logistic Regression - accuracy_train: 0.941
     Logistic Regression - accuracy_test: 0.9006
     ```
   - Random Forest
     ```
     Random Forest - accuracy_train: 0.7256
     Random Forest - accuracy_test: 0.6904
     ```
   
2. Word2Vec feature extraction, 80/20 data split, VADER labeling
   - Support Vector Machine(SVM)
     ```
     Support Vector Machine - accuracy_train: 0.7842
     Support Vector Machine - accuracy_test: 0.7536
     ```
   - Logistic Regression
     ```
     Logistic Regression - accuracy_train: 0.8138
     Logistic Regression - accuracy_test: 0.7974
     ```
   - Random Forest
     ```
     Random Forest - accuracy_train: 0.88555
     Random Forest - accuracy_test: 0.7844
     ```
3. TF-IDF feature extraction, 70/30 data split, TextBlob labeling
   - Support Vector Machine(SVM)
     ```
     Support Vector Machine - accuracy_train: 0.9866285714285714
     Support Vector Machine - accuracy_test: 0.8705333333333334
     ```
   - Logistic Regression
     ```
     Logistic Regression - accuracy_train: 0.9397142857142857
     Logistic Regression - accuracy_test: 0.8945333333333333
     ```
   - Random Forest
     ```
     Random Forest - accuracy_train: 0.7335428571428572
     Random Forest - accuracy_test: 0.6878666666666666
     ```
