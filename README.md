# 📚 Book Genre Classification Using Deep Learning

## 🧩 Problem Statement

With the exponential growth of digital books, it's becoming increasingly important to categorize them efficiently. However, many books are missing genre tags, making it hard to organize and recommend them properly.

This project aims to solve that by **automatically classifying books into genres** based on their **descriptions or titles** using Deep Learning techniques.

---

## 💡 Project Explanation

In this project, we use Natural Language Processing (NLP) and Deep Learning (specifically, LSTM neural networks) to classify books into genres such as **Romance**, **Mystery**, **Fantasy**, **History**, and **Fiction**.

### 🔨 Steps Involved:

1. **Data Preprocessing**:
   - Load a dataset of books.
   - Clean the text data by removing special characters, converting to lowercase, and removing stopwords.
   - If a `description` column is missing, the `title` is used as a fallback.

2. **Genre Assignment**:
   - For demonstration purposes, genre labels are assigned based on keywords in the book title (e.g., "magic" = Fantasy).

3. **Text Vectorization**:
   - Use Tokenizer to convert text into sequences of integers.
   - Pad sequences to ensure consistent input size.

4. **Model Building**:
   - Use an LSTM model to capture the sequential nature of language.
   - Compile and train the model on training data.

5. **Evaluation**:
   - Evaluate the model using accuracy, confusion matrix, and classification report.
   - Predict genre on custom input descriptions.

### 🤖 Technologies Used:

- Python
- TensorFlow / Keras
- Scikit-learn
- NLTK
- Pandas / NumPy
- Matplotlib / Seaborn

---

## 📂 Dataset

You can use this public dataset from Kaggle:

**📎 Dataset Title:** [Books Dataset](https://www.kaggle.com/datasets/zygmunt/goodbooks-10k)  
**Link:** https://www.kaggle.com/datasets/zygmunt/goodbooks-10k

Or you can use any `.csv` file that contains at least the following columns:
- `title` (used to simulate or generate genres)
- `description` (optional but ideal for better accuracy)

---

## ✨ Example

**Input**:
