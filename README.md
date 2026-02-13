## 📧 SMS/Email Spam Classifier
An end-to-end Machine Learning web application that predicts whether a given message is Spam or Ham (Legitimate) using Natural Language Processing (NLP).
### 🚀 Live Demo
Check out the live app here: https://sms-spam-classifier-yash.streamlit.app/
### 🧐 Overview
This project focuses on the classification of text messages into two categories. It utilizes a Multinomial Naive Bayes classifier, which is highly effective for text-based datasets. The app provides a simple user interface where anyone can paste a message and get an instant prediction with high accuracy.
### 🛠️ Tech Stack
Language: Python
Frontend: Streamlit
Machine Learning: Scikit-learn
NLP Library: NLTK
Data Handling: Pandas & NumPy
### 📊 Exploratory Data Analysis (EDA)
Before training the model, I performed extensive EDA to understand the data:
Feature Engineering: Created new features like num_characters, num_words, and num_sentences to analyze message structure.
Visualization: Used Pair Plots and Heatmaps to find correlations between features.
Word Clouds: Generated Word Clouds for both Spam and Ham to identify the most frequent "trigger" words.
### 🧹 Data Preprocessing
To prepare the text for the model, I built a pipeline that performs:
Tokenization: Breaking sentences into individual words.
Lowercasing: Converting all text to lowercase for uniformity.
Removing Special Characters: Cleaning the text of punctuation.
Removing Stopwords & Punctuation: Filtering out common words (like "the", "is", "at") that don't add predictive value.
Stemming: Reducing words to their root form (e.g., "dancing" becomes "danc").
Vectorization: Using TF-IDF Vectorizer to convert text into numerical format.
### 📂 Project Structure
#### ├── app.py             # Main Streamlit application file
#### ├── model.pkl          # Trained Naive Bayes model
#### ├── vectorizer.pkl     # TF-IDF Vectorizer object
#### ├── requirements.txt   # List of dependencies for deployment
#### └── README.md          # Project documentation
