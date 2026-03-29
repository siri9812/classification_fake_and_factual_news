# 📰 Fake News Detection using NLP & Machine Learning

## 🌍 Setting the Scene

Imagine working as a data analyst for a social media company that is increasingly concerned about the spread of **fake news** on its platform. The rise of misinformation can mislead users, influence public opinion, and reduce trust in reliable sources.

To tackle this issue, the company has assigned you to investigate how fake news can be recognized and to develop a method for identifying it automatically.

In this project, we:

* Explore and clean the dataset
* Analyze linguistic patterns in news articles
* Apply Natural Language Processing (NLP) techniques
* Build machine learning models to classify news as **Fake** or **Factual**
* Visualize insights and communicate findings effectively

---

## 📂 Dataset

The dataset used:

```
fake_new_data.csv
```

### Features:

* `text` → News article content
* `fake_or_factual` → Label (Fake News / Factual News)

---

## ⚙️ Installation

Install required libraries:

```bash
pip install pandas matplotlib seaborn spacy nltk gensim scikit-learn vaderSentiment
```

Download required resources:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

Download spaCy model:

```bash
python -m spacy download en_core_web_sm
```

---

## 🚀 Project Workflow

### 1. 📊 Exploratory Data Analysis (EDA)

* Analyze dataset structure
* Visualize distribution of fake vs factual news
* Identify class imbalance

---

### 2. 🧠 NLP Analysis

Using **spaCy**:

* Tokenization
* Part-of-Speech (POS) tagging
* Named Entity Recognition (NER)

Compare:

* Token usage
* POS distributions
* Named entities between fake and factual news

---

### 3. 🧹 Text Preprocessing

* Remove unwanted patterns (e.g., location prefixes)
* Convert text to lowercase
* Remove punctuation
* Remove stopwords
* Tokenize text
* Lemmatize words

---

### 4. 📈 N-gram Analysis

* Extract most common:

  * Unigrams
  * Bigrams
* Visualize frequent terms

---

### 5. 😊 Sentiment Analysis

Using **VADER Sentiment Analyzer**:

* Assign sentiment scores
* Classify into:

  * Positive
  * Neutral
  * Negative
* Compare sentiment across fake and factual news

---

### 6. 🧩 Topic Modeling

#### 🔹 Latent Dirichlet Allocation (LDA)

* Discover hidden topics in fake news
* Use coherence scores to determine optimal number of topics

#### 🔹 Latent Semantic Analysis (LSA)

* Apply TF-IDF transformation
* Extract topics using LSI model

---

### 7. 🤖 Machine Learning Models

#### Feature Engineering:

* Convert text into numerical format using **CountVectorizer**

#### Models Used:

* Logistic Regression
* SGD Classifier (Linear model similar to SVM)

#### Evaluation Metrics:

* Accuracy Score
* Precision, Recall, F1-score

---

## 📊 Results & Insights

* Linguistic patterns differ between fake and factual news
* Fake news often shows distinct entity and word usage patterns
* Sentiment distribution varies across categories
* Machine learning models can effectively classify news after preprocessing

---

## 📁 Project Structure

```
├── fake_new_data.csv
├── code.ipynb
└── README.md
```

---

## 🔮 Future Improvements

* Implement deep learning models (LSTM, BERT)
* Perform hyperparameter tuning
* Use larger and more diverse datasets
* Deploy as a web application (Flask/Streamlit)
* Add real-time fake news detection

---

## 📌 Conclusion

This project demonstrates how **Natural Language Processing** and **Machine Learning** can be combined to detect fake news. By leveraging text patterns, sentiment, and topic modeling, we can build systems that help reduce misinformation on social media platforms.

---

## 📄 License

This project is licensed under the MIT License.

