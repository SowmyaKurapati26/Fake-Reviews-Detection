# 🕵️‍♂️ Fake Reviews Detection

## 📌 Problem Statement

Online platforms often suffer from fake reviews that mislead customers.
The goal of this project is to build a machine learning model that can automatically identify whether a review is:

* **CG (Computer Generated)** → Fake review
* **OR (Original Review)** → Genuine human-written review

The model analyzes the review text and predicts whether it is fraudulent or authentic.

---

## 📊 Dataset Description

The dataset consists of:

* **20,000 fake (computer-generated) reviews**
* **20,000 real (human-written) reviews**

Each review contains:

* Review text
* Rating
* Label (CG or OR)
* Product category (e.g., Home, Sports, Office, etc.)

---

## ⚙️ Technologies & Libraries Used

* **Data Handling:** Numpy, Pandas
* **Visualization:** Matplotlib, Seaborn
* **Text Processing:** NLTK, String, Warnings
* **Machine Learning (Scikit-learn):**

  * Model selection & preprocessing tools
  * Classification algorithms (various)

---

## 🧹 Text Preprocessing Steps

To improve model performance, the review text is cleaned and standardized using:

* Removing punctuation
* Converting text to lowercase
* Removing stopwords (common words like "the", "is")
* Removing digits
* Stemming (reducing words to root form)
* Lemmatization (converting words to meaningful base form)

---

## 🔢 Feature Engineering

Text data is converted into numerical format using:

* **Bag of Words (CountVectorizer)**
* **TF-IDF (Term Frequency–Inverse Document Frequency)**

These techniques help the model understand word importance and frequency.

---

## 🤖 Machine Learning Models Used

The following classification algorithms were trained and evaluated:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Classifier (SVC)
4. Decision Tree
5. Random Forest
6. Multinomial Naive Bayes

---

## 📈 Model Performance

| Model                     | Accuracy        |
| ------------------------- | --------------- |
| Support Vector Classifier | **~88% (Best)** |
| Logistic Regression       | ~86%            |
| Random Forest             | ~84%            |
| Naive Bayes               | ~84%            |
| Decision Tree             | ~73%            |
| KNN                       | ~58% (Lowest)   |

### 🏆 Key Insight:

* **SVC performed the best**, making it the most reliable model for detecting fake reviews.
* Simpler models like **KNN struggled** with this task due to the complexity of text data.

---

## ✅ Conclusion

This project demonstrates how machine learning can effectively detect fraudulent reviews by analyzing writing patterns.
It highlights that **computer-generated reviews exhibit distinct characteristics** that models can learn and identify with high accuracy.

---
