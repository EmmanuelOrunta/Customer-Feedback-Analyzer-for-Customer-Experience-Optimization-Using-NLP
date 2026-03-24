# 📊 Customer Feedback Sentiment Analysis & Churn Prediction

## 📌 Project Overview

This project analyzes customer feedback from Twitter to determine sentiment (positive or negative) and predict potential customer churn risk. Using Natural Language Processing (NLP) and Machine Learning techniques, the system processes raw text data, extracts meaningful features, and builds a classification model to generate actionable business insights.

The goal is to help organizations proactively identify dissatisfied customers and improve customer experience strategies.

---

## 🚀 Key Features

- Text preprocessing and cleaning (removal of URLs, symbols, and noise)  
- Stopword removal to improve model performance  
- Rule-based sentiment labeling  
- TF-IDF vectorization for feature extraction  
- Logistic Regression model for classification  
- Churn risk prediction based on sentiment  
- Data visualization using charts and word clouds  

---

## 🧠 Technologies Used

- Python  
- Pandas & NumPy  
- NLTK (Natural Language Processing)  
- Scikit-learn (Machine Learning)  
- Matplotlib & Seaborn (Visualization)  
- WordCloud  

---

## 📂 Dataset

The dataset used is a Twitter Customer Support dataset (`twcs.csv`), containing real customer interactions which was gotten from kaggle.

### Data Preparation:
- Filtered only customer messages (`inbound = True`)  
- Selected relevant text column  
- Removed missing values  
- Sampled 50,000 records for performance  

---

## ⚙️ Project Workflow

### 1. Data Cleaning
- Convert text to lowercase  
- Remove URLs and non-alphabetic characters  

### 2. Text Preprocessing
- Remove stopwords (e.g., "the", "is", "and")  
- Reduce noise and improve feature quality  

### 3. Sentiment Labeling
- Applied rule-based labeling using predefined negative keywords  
- Classified text into:
  - **Positive**
  - **Negative**

### 4. Feature Extraction
- Used **TF-IDF (Term Frequency - Inverse Document Frequency)**  
- Converts text data into numerical format so machine learning models can understand it
- Transforms sentences into vectors (numbers) 
- Limited to top 5000 features  

### 5. Model Training
- Split dataset into training (80%) and testing (20%)  
- Used **Logistic Regression** for classification  
- Trained model to learn patterns in customer feedback  

### 6. Model Evaluation
- Evaluated using:
  - Accuracy score  
  - Classification report (precision, recall, F1-score)  

### 7. Churn Risk Prediction
This section of the code segments each of the sentinent into High Risk or Low Risk.. Basically saying that if a comment or feedback is negative, classify the review as a High Risk
- Negative sentiment → **High Risk**  
- Positive sentiment → **Low Risk**  

### 8. Visualization
- Sentiment distribution chart  
- Word cloud of common complaints  

---

## 📈 Results & Insights

- Successfully classified customer sentiment using machine learning  
- Identified common complaint patterns through word cloud analysis  
- Enabled churn risk detection based on negative sentiment  

This demonstrates how raw customer data can be transformed into actionable insights.

---

## ⚠️ Limitations

- Sentiment labels are rule-based (not manually labeled)  
- Model may not capture context (e.g., sarcasm or negation like "not bad")  
- Limited vocabulary due to TF-IDF feature cap  

---

## 🔮 Future Improvements

- Use advanced NLP models (e.g., BERT, VADER, TextBlob)  
- Implement deep learning for better context understanding  
- Use real labeled datasets  
- Build an interactive dashboard (Power BI / Streamlit)  
- Add customer-level churn tracking  

---

## 💡 Business Use Case

This project can be applied in:

- Insurance  
- Banking  
- Telecommunications  
- E-commerce  

Organizations can:
- Detect dissatisfied customers early  
- Improve service delivery  
- Reduce churn  
- Enhance customer experience  

---
Note: This project was used to practice basic machine learning skills and models..
