# 📰 Fake News Prediction

<p align="center">  
  <strong>A Machine Learning pipeline to detect fake news using Natural Language Processing (NLP) techniques.</strong>  
</p>  

---

## 📖 Overview

The rapid spread of misinformation and fake news poses risks to society—impacting politics, public opinion, and daily decision-making.

**Fake News Prediction** is a **Python-based ML project** that:

* 🧹 **Cleans and preprocesses** raw news data (author, title, text)
* 🔠 Converts text into numerical features using **TF-IDF Vectorization**
* 🤖 Trains a **Logistic Regression classifier** to distinguish real vs. fake news
* 📊 Evaluates accuracy on training & test data
* 📝 Provides **prediction outputs with probabilities**

---

## 🎯 Use Cases

* 🚨 **Fake News Detection** → Flag unreliable or deceptive news content
* 📰 **Media Monitoring** → Assist fact-checkers in analyzing large volumes of articles
* 🎓 **Research & Education** → Demonstrate NLP + ML in misinformation studies
* 💻 **Prototype for Applications** → Base model for fact-checking tools

---

## 🛠️ Technology Stack

| Layer                  | Tools & Libraries                      |
| ---------------------- | -------------------------------------- |
| **Programming**        | Python 🐍                              |
| **Data Handling**      | pandas, numpy                          |
| **NLP Processing**     | nltk (stopwords, stemming)             |
| **Feature Extraction** | TF-IDF Vectorizer                      |
| **Machine Learning**   | Logistic Regression (scikit-learn)     |
| **Evaluation**         | Accuracy Score, Prediction Probability |

---

## 🧭 Workflow

```mermaid
flowchart TB
  A[📥 Raw News Dataset] --> B[🧹 Text Preprocessing (Cleaning + Stemming)]
  B --> C[🔡 TF-IDF Vectorization]
  C --> D[🤖 Train Logistic Regression Model]
  D --> E[📊 Evaluate Model & Predict Labels]
```

---

## 📜 Core Components

| File / Dataset                                         | Description                                                                    |
| ------------------------------------------------------ | ------------------------------------------------------------------------------ |
| [`fake_news_prediction.py`](./fake_news_prediction.py) | Main script: preprocessing → feature engineering → model training → evaluation |
| `train.csv`                                            | Dataset containing news articles (`author`, `title`, `label`)                  |
| **Output**                                             | Training/Test Accuracy, Prediction Probability for sample news                 |

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/tanmaypant/Fake_news_prediction.git
cd Fake_news_prediction
```

### 2️⃣ Install Dependencies

```bash
pip install pandas numpy scikit-learn nltk
```

### 3️⃣ Run the Script

```bash
python fake_news_prediction.py
```

### ✅ Sample Output

```
Training Accuracy: 0.96  
Test Accuracy: 0.93  
Sample Prediction: REAL (Probability: 0.742)
```

---

## 📁 Project Structure

```plaintext
Fake_news_prediction/
├── fake_news_prediction.py   # ML pipeline (preprocessing → training → evaluation)
├── train.csv                 # Dataset with author, title, and labels
└── README.md                 # Documentation
```

---

## 🔮 Future Roadmap

* 🌐 Add **more ML models** (Random Forest, SVM, XGBoost)
* 🤖 Explore **Deep Learning (LSTM, BERT)** for contextual predictions
* 📊 Provide **advanced evaluation metrics** (Precision, Recall, F1, Confusion Matrix)
* 🖥️ Build an **interactive Streamlit/Flask web app** for real-time predictions

---

## 🌟 Closing Note

> *“In an era of information overload, truth matters more than ever.
> This project helps distinguish **fact from fiction**—one article at a time.”* 📰✨
