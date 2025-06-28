# 📰 <h1>Fake News Detection  </h1>
Detecting fake vs real news articles using NLP and Machine Learning techniques  

---

## 📌 Introduction  

In today's fast-paced digital world, news spreads in seconds — but not all of it is true. Fake news has become a real problem, capable of shaping public opinion, spreading fear, and even influencing major events. 
This project tackles the challenge of automated fake news detection using Natural Language Processing (NLP) and Machine Learning.

By analyzing the content of news articles, our model learns to distinguish between real and fake news with high accuracy (98.57%) — helping to combat the spread of disinformation.

---

## 📂 Dataset  
The dataset is a combination of two CSV files containing news articles:  
- `Fake.csv.zip` — labeled as fake news (`label = 0`)  
- `True.csv.zip` — labeled as real news (`label = 1`)  

Each dataset includes the full text of news articles and their corresponding labels.

---

## 🔍 Methodology  
- Load and merge datasets  
- Clean and preprocess text:  
  - Lowercase, remove punctuation and numbers  
  - Remove stopwords and apply stemming  
- Split data into training (80%) and testing (20%) sets with stratification  
- Extract features using TF-IDF vectorizer (max 5000 features)  
- Train Logistic Regression classifier  
- Evaluate model performance on test data using accuracy, precision, recall, and F1-score  

---

## ✅ Results
- Accuracy: ~98.57%
- Balanced precision and recall across both classes
- Model performs well in detecting both fake and real news

---

## 📊 Visualizations  
- **Class Distribution:** Count plot of fake vs. real news samples  
- **Word Cloud:** Visual representation of frequent words in fake news articles  

---

## ▶️ How to Run  
1. Clone the repo or download the notebook/script  
2. Place the `Fake.csv.zip` and `True.csv.zip` files in the project directory  
3. Run the script or notebook to train the model and view performance metrics  
4. View generated plots (class distribution, word cloud)  

---

## 🧰 Requirements  
- Python 3.x  
- pandas  
- numpy  
- nltk  
- scikit-learn  
- matplotlib  
- seaborn  
- wordcloud  

Install all with:
```bash
pip install -r requirements.txt


## 🚀 Technologies Used  
- Python  
- Pandas & NumPy  
- NLTK (for stopwords and stemming)  
- Scikit-learn (for TF-IDF and Logistic Regression)
