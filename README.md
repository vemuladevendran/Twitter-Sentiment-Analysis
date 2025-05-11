# 🐦 Twitter Sentiment Analysis using Logistic Regression

This project performs sentiment analysis on a dataset of 1.6 million tweets using **Logistic Regression**. The objective is to classify tweets as either **positive** or **negative** based on their content using Natural Language Processing (NLP) techniques.

---

## 📌 Features

- Uses the [Sentiment140 dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)
- Preprocessing includes:
  - Cleaning and lowercasing
  - Removing stopwords
  - Tokenization
  - Stemming (⚠️ Takes ~30+ minutes for 1.6M tweets)
- TF-IDF vectorization
- Model training using Logistic Regression
- Accuracy and Confusion Matrix for evaluation

---

## 🚀 Getting Started

### ✅ Run with Google Colab (Recommended)

> **Why Google Colab?**  
> Easy setup, no local installations, and free GPU options!

### 📦 Required Installations

Once the notebook is loaded in Google Colab, run the following to install dependencies:

```bash
!pip install numpy pandas scikit-learn matplotlib seaborn nltk kaggle
```

## 🔑 Setting Up Kaggle API Key

To download the dataset from Kaggle, you’ll need to upload your `kaggle.json` API key.

### 📝 Steps to Download:

1. Go to [Kaggle.com](https://www.kaggle.com/).
2. Click on your profile icon → **Account**.
3. Scroll down to the **API** section.
4. Click **"Create New API Token"**.
5. A file named `kaggle.json` will be downloaded automatically.

### 📂 Upload or Place the File

- If using **Google Colab**, upload the `kaggle.json` file using the file upload panel.
- If running locally, place the file in your project root directory.

### 📁 Setup Code (run in Colab):

```python
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
````

## 🕒 Note on Stemming Process

⚠️ **Warning**:  
The stemming step processes **1.6 million tweets** and may take **at least 30 minutes** to complete.

Please be patient and **do not interrupt** this process.

---

## 📈 Output

After running the notebook, you will get:

- ✅ Trained **Logistic Regression** model  
- 📊 **Accuracy score**
