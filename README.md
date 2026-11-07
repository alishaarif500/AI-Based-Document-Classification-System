 # AI-Based-Document-Classification-System

An end-to-end Natural Language Processing (NLP) and Machine Learning** project that automatically classifies news articles into five predefined categories: Business, Entertainment, Politics, Sport, and Tech.
Developed using the BBC News dataset, the system demonstrates a complete text-classification pipeline, including dataset cleaning, duplicate removal, text preprocessing, feature extraction, model training, evaluation, and interactive prediction.
 Key Features
- Dataset Preparation:Processes 2,225 BBC news articles and removes duplicates, resulting in 2,127 unique documents.
- Text Preprocessing: Applies lowercasing, punctuation and digit removal, tokenization, stop-word removal, and lemmatization.
- Feature Extraction: Uses TF-IDF vectorization with unigrams and bigrams, limited to 5,000 features.
- Machine Learning Models: Implements and compares Logistic Regression and Multinomial Naive Bayes.
- *Model Evaluation:** Measures accuracy, precision, recall, and F1-score, supported by classification reports and confusion matrices.
- Interactive Prediction:Allows users to enter news articles, select a trained model, and receive predicted categories with probability scores.
  Web Deployment:Provides a Streamlit application for real-time document classification.
 Model Performance
The current notebook reports the following test accuracies:
| Algorithm | Accuracy |
|---|---:|
| Logistic Regression | 97.65% |
| Multinomial Naive Bayes | 98.12% |
 Technologies Used
Python, Pandas, NumPy, NLTK, Scikit-learn, TF-IDF, Matplotlib, Seaborn, Pickle, and Streamlit.
 Project Objective
To demonstrate practical expertise in Natural Language Processing, supervised Machine Learning, text analytics, model evaluation, and interactive AI application development.

This project showcases the complete journey from raw textual data to an intelligent document classification application.
