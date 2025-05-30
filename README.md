
  
# Amazon Product Review Sentiment Analysis

This project performs sentiment analysis on a subset of Amazon product reviews. The goal is to classify reviews into **positive**, **neutral**, or **negative** sentiments based on the review text.

---

## What I Learned

- Text preprocessing techniques: cleaning, tokenization, stopword removal, and lemmatization
- How to use NLTK’s `PunktSentenceTokenizer` and `TreebankWordTokenizer` to avoid tokenizer errors in Google Colab
- Feature extraction using TF-IDF vectorization
- Building a machine learning model with Logistic Regression for text classification
- Evaluating model performance with classification reports and confusion matrices
- Uploading and handling datasets in Google Colab

---

## Dataset

- The dataset is a small subset of Amazon product reviews with columns including `Text` and `Score`.
- Sentiment labels are created based on the score:
  - Scores 1 and 2: **Negative**
  - Score 3: **Neutral**
  - Scores 4 and 5: **Positive**

---

## How the Program Works (Step-by-step)

1. **Upload Dataset**: Upload your CSV file (`Reviews_small_demo.csv`) into the Colab notebook.
2. **Import Libraries & Download Resources**: Installs and sets up necessary packages like NLTK and scikit-learn.
3. **Load Data**: Loads the CSV file into a pandas DataFrame.
4. **Label Sentiment**: Maps numerical review scores to sentiment categories (positive, neutral, negative).
5. **Text Preprocessing**:
    - Converts text to lowercase
    - Removes special characters and punctuation
    - Tokenizes sentences using `PunktSentenceTokenizer`
    - Tokenizes words using `TreebankWordTokenizer` (this avoids the common `punkt_tab` error in Colab)
    - Removes stopwords
    - Lemmatizes words to their base forms
6. **TF-IDF Vectorization**: Converts cleaned text into numerical features.
7. **Train-Test Split**: Splits data into training and testing sets.
8. **Train Model**: Trains a Logistic Regression classifier on training data.
9. **Evaluate Model**: Prints classification report and visualizes confusion matrix for model predictions.

---

## How to Run

- Open the provided Google Colab notebook.
- Upload the `Reviews_small_demo.csv` dataset when prompted.
- Run all cells sequentially.
- Check output cells for model accuracy and evaluation metrics.

---

## Certificate

Add your Coursera Data Science course certificate link here:
https://www.coursera.org/account/accomplishments/verify/W2VQGBG5XJ7H?utm_source=ios&utm_medium=certificate&utm_content=cert_image&utm_campaign=sharing_cta&utm_product=course

---

## Notes

- This project demonstrates practical skills learned from the Coursera Data Science crash course.
- The use of explicit tokenizers ensures the notebook runs smoothly on Google Colab without NLTK resource errors.
- This repository is ideal for showcasing beginner to intermediate data science skills.

---

# Author

**Vaishnavi gopi**  
Connect with me on https://www.linkedin.com/in/vaishnavi-gopi-183653243?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app 

---

