# AI-Based Document Classification System

A text-classification project that sorts BBC news articles into five categories (business, entertainment, politics, sport, tech) using TF-IDF features with Logistic Regression and Multinomial Naive Bayes, built with Python and scikit-learn.

## Overview

The notebook covers a full classical NLP pipeline: loading the BBC News dataset, removing duplicates, cleaning and normalising text, extracting TF-IDF features, training two classifiers, comparing them with classification reports, and predicting the category of new text with class probabilities.

## Dataset

- **Source:** BBC News articles (2,225 articles), downloaded in the notebook.
- **Cleaning:** 98 duplicate rows were removed, leaving **2,127** unique articles.
- **Classes after cleaning:** sport 505, business 503, politics 403, entertainment 369, tech 347.

## Methodology

1. Remove duplicate articles.
2. Preprocess text with NLTK: lowercasing, removing punctuation and digits, tokenisation, stop-word removal and lemmatisation.
3. Convert text to TF-IDF vectors (5,000 features).
4. Split the data 80/20: 1,701 training and 426 test articles.
5. Train Logistic Regression and Multinomial Naive Bayes.
6. Evaluate with precision, recall, F1-score and confusion matrices.
7. Predict the category of custom text and show the probability for each class.

## Results

Evaluated on the 426 held-out test articles:

| Model | Accuracy |
|---|---|
| Logistic Regression | 0.9765 |
| Multinomial Naive Bayes | 0.9812 |

Per-class F1-scores are between 0.96 and 1.00 for both models. Politics and business were the most frequently confused categories (lowest F1 at 0.96-0.97).

## Limitations

- The dataset is small, and its categories are fairly distinct in vocabulary, which makes the task easier than classifying text from mixed sources.
- Results come from a single random split with 426 test articles, so the small accuracy difference between the two models should not be over-interpreted.
- The models were not tested on news from other publishers or time periods.
- In a sample prediction, Logistic Regression returned a low-confidence result (about 53%), so probabilities should be read with care on short or unusual text.

## Future Improvements

- Use cross-validation and test on an independent news dataset.
- Compare with a linear SVM or a transformer-based model.
- Add the Streamlit app and saved models to the repository (the notebook generates the app script, but it is not included here).

## Project Files

| File | Description |
|---|---|
| `AI_Based_Document_Classification_System.ipynb` | Main notebook: preprocessing, training, evaluation, interactive prediction |
| `ai_based_document_classification_system (1).py` | Python export of the notebook |

## How to Run

The notebook was built in Google Colab and downloads the dataset and NLTK resources, so it needs an internet connection.

**Google Colab (recommended):** upload the notebook and run all cells.

**Locally:**

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn jupyter
jupyter notebook AI_Based_Document_Classification_System.ipynb
```

## Technologies

Python · Pandas · NumPy · NLTK · scikit-learn (TF-IDF, Logistic Regression, Naive Bayes) · Matplotlib · Seaborn · Google Colab

## Author

**Alisha Arif** · [GitHub](https://github.com/alishaarif500) · [LinkedIn](https://linkedin.com/in/alisha-arif-22aa42386/)
