#  Sentiment Analysis on Product Reviews

##  Overview
This project uses **Machine Learning** to classify product reviews as **Positive (1)** or **Negative (0)**.  
We use text preprocessing, feature extraction with **TF-IDF**, and multiple classification algorithms including:
- Logistic Regression
- Naive Bayes

The dataset contains product reviews with their corresponding sentiment labels.  
We train our model on historical data and then predict the sentiment of new, unseen reviews.

---

##  Dataset
- **Source**: Amazon Product Reviews (CSV file)
- **Features**:
  - `Review`: The text of the product review
  - `Sentiment`: The label (Positive = 1, Negative = 0)
- **Data Size**: ~30,000+ reviews after preprocessing

---

## ⚙️ Steps Performed
1. **Load Dataset**  
   Imported CSV file using `pandas`.

2. **Data Cleaning & Preprocessing**  
   - Lowercasing text  
   - Removing stopwords  
   - Handling missing values  
   - Converting sentiments to binary (1 for Positive, 0 for Negative)  

3. **Feature Extraction (TF-IDF)**  
   - Used `TfidfVectorizer` to convert text into numerical vectors.
   - Removed common stopwords, applied lowercase conversion, and set `max_df=0.9` to ignore overly frequent terms.

4. **Model Training**  
   - **Logistic Regression** for high accuracy prediction.  
   - **Naive Bayes** for faster computation and probabilistic classification.

5. **Model Evaluation**  
   - Measured **accuracy**, **precision**, **recall**, and **F1-score**.
   - Logistic Regression achieved ~95% accuracy.

6. **Custom Predictions**  
   - Input any custom review and classify it as Positive (1) or Negative (0).

7. **Visualization**  
   - Word clouds for most frequent positive and negative words.
   - Sentiment distribution bar chart.

---

## 📊 Results
| Model              | Accuracy |
|--------------------|----------|
| Logistic Regression| 95%      |
| Naive Bayes        | 93%      |

---





