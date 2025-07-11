# Disaster Tweet Classification

---

## Project Overview

This project is a solution for the "Real or Not? NLP with Disaster Tweets" Kaggle competition. The goal is to build a machine learning model capable of predicting whether a given tweet is a real disaster (binary class 1) or not (binary class 0), based on its text content and other metadata.

This project serves as an excellent starting point in Natural Language Processing (NLP) and text classification, covering essential steps from data understanding to model building and submission.

---
## Repository Contents

* `notebook.ipynb` (or similar): The Jupyter notebook containing all steps for data analysis, preprocessing, feature engineering, model building, and evaluation.
* `train.csv`: The original training dataset from Kaggle.
* `test.csv`: The original test dataset from Kaggle.
* `sample_submission.csv`: An example submission file format required by Kaggle.
* `submission.csv`: The final submission file generated by my model, uploaded to Kaggle.

---
## Methodology

1.  **Exploratory Data Analysis (EDA):** Examining the dataset to understand its structure, missing values, and target class distribution.
2.  **Missing Data Handling:** Addressing missing values in `keyword` and `location` columns.
3.  **Text Preprocessing:**
    * Lowercase conversion.
    * Removal of URLs, hashtags (keeping the word), and @mentions.
    * Removal of punctuation, numbers, and emojis.
    * Stop word removal.
    * Lemmatization.
4.  **Feature Engineering:**
    * Extracting new features from the raw text like tweet length, word count, punctuation count, and uppercase letter ratio.
    * Creating binary features indicating the presence or absence of keywords and locations.
5.  **Text Vectorization:** Utilizing **TF-IDF Vectorizer** to transform processed text into numerical representations suitable for machine learning models.
6.  **Feature Combination:** Merging TF-IDF features with the engineered numerical features.
7.  **Model Building and Training:** Employing a **Logistic Regression** model (other models like Naive Bayes or SVM could be explored) for training on the processed and transformed data.
8.  **Evaluation:** Assessing model performance using **F1-Score** on a validation set, which is the primary competition metric.
9.  **Submission File Generation:** Creating the `submission.csv` file in the required format for Kaggle.
---

## Tools and Libraries Used

* **Python**
* **Pandas:** For data manipulation and analysis.
* **NumPy:** For numerical operations and array handling.
* **NLTK (Natural Language Toolkit):** For text preprocessing (stopwords, lemmatization).
* **Scikit-learn:** For text vectorization (TF-IDF) and machine learning model building (Logistic Regression).
* **Jupyter Notebook:** For interactive development.

---
## Results and Achievements

* Achieved an initial F1-Score of **[YOUR BEST F1-SCORE FROM KAGGLE]** on the Kaggle leaderboard.
* Demonstrated significant performance improvement through meticulous text preprocessing and additional feature engineering.

