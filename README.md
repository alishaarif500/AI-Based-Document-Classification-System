

# 🤖 AI-Based Document Classification System

**An NLP and Machine Learning project that automatically classifies BBC News articles into five categories using TF-IDF feature extraction, Logistic Regression, and Multinomial Naive Bayes.**

## 📌 Overview

The AI-Based Document Classification System is an end-to-end Natural Language Processing (NLP) and supervised Machine Learning project designed to automatically categorize news articles into predefined topics.

Using the BBC News dataset, the system processes and cleans textual data, removes duplicate articles, extracts meaningful text features using TF-IDF, and trains two machine learning classification models: Logistic Regression and Multinomial Naive Bayes.

The project also supports custom text predictions, allowing users to classify new articles and view their predicted categories with class probability scores.

## 🎯 Project Objectives

The primary objectives of this project are to:

- Develop an automated system for classifying news articles into predefined categories using Natural Language Processing.
- Apply text preprocessing techniques to clean, normalize, and prepare unstructured textual data.
- Transform text into meaningful numerical representations using TF-IDF feature extraction.
- Implement and compare Logistic Regression and Multinomial Naive Bayes for multi-class text classification.
- Evaluate model performance using accuracy, precision, recall, F1-score, and confusion matrices.
- Identify the better-performing classification model through comparative evaluation.
- Enable automated categorization of new text with predicted labels and class probability scores.

## ✨ Key Features

- **Multi-Class Classification:** Categorizes news articles into five topics: Business, Entertainment, Politics, Sport, and Tech.
- **Text Preprocessing:** Cleans and prepares text by removing unnecessary characters, stop words, and duplicates.
- **NLTK-Based Processing:** Uses tokenization, lowercasing, and lemmatization.
- **TF-IDF Feature Extraction:** Converts text into numerical features using unigram and bigram representations.
- **Machine Learning Models:** Implements Logistic Regression and Multinomial Naive Bayes.
- **Model Evaluation:** Evaluates performance using accuracy, precision, recall, F1-score, classification reports, and confusion matrices.
- **Custom Text Prediction:** Allows users to enter new text and obtain a predicted category.
- **Probability Analysis:** Displays class probability scores for predictions.
- **Model Comparison:** Compares both classifiers to identify the better-performing model.

## 📊 Dataset

This project uses the **BBC News Articles Dataset**, containing news articles from five categories.

### Dataset Summary

| Description | Count |
|---|---:|
| Original articles | 2,225 |
| Duplicate articles removed | 98 |
| Unique articles | 2,127 |
| Training samples (80%) | 1,701 |
| Testing samples (20%) | 426 |
| Maximum TF-IDF features | 5,000 |

### Category Distribution

| Category | Articles |
|---|---:|
| Sport | 505 |
| Business | 503 |
| Politics | 403 |
| Entertainment | 369 |
| Tech | 347 |
| **Total** | **2,127** |

The dataset is downloaded within the notebook.

## ⚙️ Methodology

The project follows a structured NLP and Machine Learning workflow:

1. **Dataset Loading:** Loads the BBC News dataset.
2. **Duplicate Removal:** Identifies and removes duplicate articles.
3. **Text Preprocessing:** Applies lowercase conversion, punctuation and digit removal, tokenization, stop-word removal, and lemmatization using NLTK.
4. **Feature Extraction:** Converts text into numerical features using TF-IDF with unigrams and bigrams, limited to 5,000 features.
5. **Data Splitting:** Divides the dataset into training (80%) and testing (20%) sets using stratified sampling.
6. **Model Training:** Trains Logistic Regression and Multinomial Naive Bayes classifiers.
7. **Model Evaluation:** Evaluates both models using classification metrics and confusion matrices.
8. **Custom Prediction:** Predicts categories for new text and provides class probability scores.

## 📈 Model Performance & Results

Both models were evaluated on **426 held-out test articles**.

### Accuracy Comparison

| Model | Accuracy |
|---|---:|
| Logistic Regression | 97.65% |
| Multinomial Naive Bayes | **98.12%** |

### Evaluation Highlights

- Both models achieved strong classification performance.
- Class-wise F1-scores ranged from 0.96 to 1.00 for both models.
- Business and Politics were the most frequently confused categories.
- Multinomial Naive Bayes achieved the highest accuracy of **98.12%**.

<details>
<summary><b>Additional Evaluation Insights</b></summary>

The models were also assessed using:

- Precision, recall, and F1-score.
- Classification reports for individual categories.
- Confusion matrices to analyze classification errors.
- Comparative evaluation to identify the better-performing model.

</details>

**Best-Performing Model:** Multinomial Naive Bayes (98.12% accuracy).

## 🛠️ Technologies & Libraries

| Category | Tools |
|---|---|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Natural Language Processing | NLTK |
| Feature Extraction | TF-IDF |
| Machine Learning | Scikit-learn |
| Data Visualization | Matplotlib, Seaborn |
| Model Serialization | Pickle |
| Development Environment | Jupyter Notebook |

## 📁 Project Structure

```text
AI-Based-Document-Classification-System/
│
├── AI_Based_Document_Classification_System.ipynb
├── .gitignore
└── README.md
```

## 🚀 Installation & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/alishaarif500/AI-Based-Document-Classification-System.git
```

### 2. Navigate to the Project Directory

```bash
cd AI-Based-Document-Classification-System
```

### 3. Install Required Libraries

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the Project

- Open `AI_Based_Document_Classification_System.ipynb`.
- Execute the notebook cells sequentially.
- Follow the workflow for data preprocessing, feature extraction, model training, and evaluation.
- Use the custom prediction functionality to classify new text.

**Note:** An internet connection is required for the initial dataset download. Required NLTK resources must also be available.

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Understanding Natural Language Processing fundamentals.
- Cleaning and preprocessing textual data using NLTK.
- Converting text into numerical representations using TF-IDF.
- Implementing supervised Machine Learning classification algorithms.
- Evaluating models using accuracy, precision, recall, and F1-score.
- Interpreting confusion matrices and class-wise classification results.
- Comparing machine learning models based on performance.
- Developing an end-to-end text classification workflow, from raw data preprocessing to custom predictions.

## 👩‍💻 Developer

**Alisha Arif**

- **GitHub:** [github.com/alishaarif500](https://github.com/alishaarif500)
- **LinkedIn:** [linkedin.com/in/alisha-arif-22aa42386](https://linkedin.com/in/alisha-arif-22aa42386)
- **Email:** [alishaarif500@gmail.com](mailto:alishaarif500@gmail.com)

---

⭐ If you find this project useful, consider giving the repository a star!

