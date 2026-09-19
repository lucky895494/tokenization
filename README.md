# tokenization
# 🔤 NLTK Sentence & Word Tokenization

## 📌 Overview

This project demonstrates the concept and implementation of **Tokenization in Natural Language Processing (NLP)** using the **NLTK (Natural Language Toolkit)** library in Python.

Tokenization is one of the fundamental steps in NLP. It involves breaking a large piece of text into smaller meaningful units called **tokens**.

This project focuses on two major types of tokenization:

* **Sentence Tokenization**
* **Word Tokenization**

The implementation is performed using a **Jupyter Notebook**.

---

## 🎯 Objectives

The main objectives of this project are:

* Understand the concept of tokenization in NLP.
* Learn how to perform sentence tokenization using NLTK.
* Learn how to perform word tokenization using NLTK.
* Understand the difference between sentence-level and word-level tokens.
* Implement tokenization on sample text using Python.

---

## 🧠 What is Tokenization?

**Tokenization** is the process of dividing text into smaller units called **tokens**.

For example:

```text
"Natural Language Processing is interesting."
```

After word tokenization:

```text
["Natural", "Language", "Processing", "is", "interesting", "."]
```

Similarly, a paragraph can be divided into individual sentences.

Tokenization is commonly used as a preprocessing step in NLP applications.

---

## ✂️ Types of Tokenization

### 1. Sentence Tokenization

Sentence tokenization divides a paragraph or large text into individual sentences.

For example:

```text
"Hello! How are you? I am learning NLP."
```

becomes:

```text
[
    "Hello!",
    "How are you?",
    "I am learning NLP."
]
```

NLTK provides the `sent_tokenize()` function for sentence tokenization.

```python
from nltk.tokenize import sent_tokenize

text = "Hello! How are you? I am learning NLP."

sentences = sent_tokenize(text)

print(sentences)
```

### Output

```text
['Hello!', 'How are you?', 'I am learning NLP.']
```

---

### 2. Word Tokenization

Word tokenization divides a sentence or text into individual words and punctuation tokens.

For example:

```text
"Python is easy to learn."
```

becomes:

```text
["Python", "is", "easy", "to", "learn", "."]
```

NLTK provides the `word_tokenize()` function for this purpose.

```python
from nltk.tokenize import word_tokenize

text = "Python is easy to learn."

words = word_tokenize(text)

print(words)
```

### Output

```text
['Python', 'is', 'easy', 'to', 'learn', '.']
```

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* **NLTK (Natural Language Toolkit)**

---

## ⚙️ Installation

Install NLTK using pip:

```bash
pip install nltk
```

Then import NLTK:

```python
import nltk
```

Depending on the NLTK version and tokenizer being used, download the required tokenizer resources:

```python
nltk.download('punkt')
```

---

## 🚀 Implementation

### Sentence Tokenization

```python
import nltk
from nltk.tokenize import sent_tokenize

nltk.download('punkt')

text = """Natural Language Processing is a branch of Artificial Intelligence.
It helps computers work with human language.
NLTK is a popular Python library for NLP."""

sentences = sent_tokenize(text)

for sentence in sentences:
    print(sentence)
```

### Word Tokenization

```python
from nltk.tokenize import word_tokenize

text = "Natural Language Processing is a branch of Artificial Intelligence."

words = word_tokenize(text)

print(words)
```

---

## 🔄 Tokenization Workflow

```text
                Raw Text
                   │
                   ▼
             ┌───────────┐
             │    NLTK   │
             └─────┬─────┘
                   │
          ┌────────┴────────┐
          ▼                 ▼
 Sentence Tokenization   Word Tokenization
          │                 │
          ▼                 ▼
     Sentences            Words
```

---

## 📊 Sentence vs Word Tokenization

| Feature  | Sentence Tokenization                 | Word Tokenization              |
| -------- | ------------------------------------- | ------------------------------ |
| Purpose  | Splits text into sentences            | Splits text into words/tokens  |
| Function | `sent_tokenize()`                     | `word_tokenize()`              |
| Input    | Paragraph/Text                        | Sentence/Text                  |
| Output   | List of sentences                     | List of words/tokens           |
| Example  | `"Hello! How are you?"` → 2 sentences | `"Hello World"` → words/tokens |

---

## 💡 Applications

Tokenization is an important preprocessing step in many NLP applications, including:

* 💬 Chatbots
* 😊 Sentiment Analysis
* 📰 Text Classification
* 🔍 Information Retrieval
* 🌐 Machine Translation
* 📄 Text Summarization
* 🤖 Natural Language Understanding
* 🧠 Machine Learning and AI

---

## 📁 Project Structure

```text
NLTK-Tokenization/
│
├── NLTK_Tokenization.ipynb
└── README.md
```

---

## 🎓 Learning Outcomes

After completing this project, you will understand:

* What tokenization is.
* Why tokenization is important in NLP.
* How to divide text into sentences.
* How to divide text into words/tokens.
* How to use NLTK's `sent_tokenize()` and `word_tokenize()` functions.
* How tokenization forms the foundation of further NLP preprocessing.

---

## 🔮 Future Scope

This project can be extended by adding other NLP preprocessing techniques such as:

* Stopword Removal
* Stemming
* Lemmatization
* Part-of-Speech (POS) Tagging
* Named Entity Recognition (NER)
* Text Classification
* Sentiment Analysis

---

## 👨‍💻 Author

**Lucky**

B.Tech Engineering Student | AI & Generative AI Enthusiast

