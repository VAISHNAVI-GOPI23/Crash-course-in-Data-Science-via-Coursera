# Amazon Product Review Sentiment Analysis

This project performs sentiment analysis on Amazon product reviews using Natural Language Processing (NLP) and Machine Learning (ML). Reviews are classified as **positive**, **neutral**, or **negative** based on their text content.

---

## What I Learned from the Coursera Data Science Crash Course

During the course, I gained practical knowledge in:
- Understanding the **data science lifecycle** from data collection to model evaluation.
- Performing **data wrangling** and **exploratory data analysis (EDA)**.
- Applying **text preprocessing techniques** like stopword removal, tokenization, and lemmatization.
- Using **vectorization (TF-IDF)** to convert text into numerical features.
- Building and evaluating a **machine learning classification model**.
- Implementing real-world projects using **Python**, **pandas**, and **scikit-learn**.

 **Course Certificate**: https://www.coursera.org/account/accomplishments/verify/W2VQGBG5XJ7H?utm_source=ios&utm_medium=certificate&utm_content=cert_image&utm_campaign=sharing_cta&utm_product=course

---

# Dataset Used

**Amazon Fine Food Reviews**  
- Source: [Kaggle Dataset](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)
- 568,000+ reviews including rating scores and text
- Columns used: `Text` (Review body) and `Score` (Rating)

---

# Technologies & Libraries

- Python
- Pandas, NumPy
- NLTK (Natural Language Toolkit)
- Scikit-learn
- Matplotlib & Seaborn
- Jupyter Notebook / Google Colab

---

# How the Program Works — Step-by-Step

1. **Dataset Upload & Loading**
   - Load the `Reviews.csv` file using pandas.
   - Keep only `Text` and `Score` columns.

2. **Data Cleaning**
   - Remove duplicates and missing values.
   - Filter scores to be between 1 and 5.

3. **Label Sentiment**
   - Convert numerical scores into sentiment labels:
     - `1-2` → Negative
     - `3` → Neutral
     - `4-5` → Positive

4. **Text Preprocessing**
   - Convert text to lowercase.
   - Remove punctuation and non-alphabetic characters.
   - Tokenize text into words.
   - Remove stopwords (like "the", "is", "and").
   - Lemmatize words to their root forms.

5. **Text Vectorization**
   - Use `TfidfVectorizer` to transform the text into numerical features.

6. **Model Training**
   - Split the data into training and test sets.
   - Train a Logistic Regression classifier.

7. **Model Evaluation**
   - Predict sentiments on the test set.
   - Evaluate performance using classification report and confusion matrix.

8. **Model Saving**
   - Save both the trained model and the vectorizer using `joblib` for future use.


---

# How to Run This Project

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload this notebook and `Reviews.csv`
3. Run the notebook step-by-step
4. Download the trained model (`sentiment_model.pkl`) and vectorizer (`tfidf_vectorizer.pkl`) if needed

---

# Future Improvements

- Add a Streamlit or Flask app for real-time review classification
- Use deep learning (LSTM, BERT) for better performance
- Expand dataset for multilingual analysis

---

# Author

**Vaishnavi gopi**  
Connect with me onhttps://www.linkedin.com/in/vaishnavi-gopi-183653243?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app 

---

