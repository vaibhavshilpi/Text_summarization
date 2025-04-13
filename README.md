# Text_summarization
This text summarization code using NLTK (Natural Language Toolkit) in Python. This approach is based on frequency of words and extracting the most relevant sentences.

This is a simple extractive text summarizer built with **pure Python**, without requiring any external libraries like `nltk`, `spacy`, or `transformers`.

It:
- Tokenizes sentences using basic punctuation.
- Uses a predefined list of English stopwords.
- Scores sentences based on word frequency.
- Returns the top N most relevant sentences as a summary.

---

## 🚀 Features

- ✅ No downloads or internet required
- ✅ No external libraries
- ✅ Lightweight and fast
- ✅ Easy to use and customize

---

## 📦 Requirements

Nothing! Just plain Python 3.

---

## 🧠 How It Works

1. Splits the text into sentences using `. ` as the delimiter.
2. Tokenizes each sentence into words, removing punctuation and stopwords.
3. Scores each sentence based on the frequency of meaningful words.
4. Returns the top `n` sentences as the summary.

---

## 🧪 Example Usage

```python
text = """
Natural language processing (NLP) is a field of artificial intelligence that focuses on the interaction between computers and humans through natural language.
The ultimate goal of NLP is to enable computers to understand, interpret, and generate human languages.
It is used in a variety of applications including speech recognition, machine translation, and sentiment analysis.
NLTK is one of the most commonly used Python libraries for NLP.
It provides easy-to-use interfaces to over 50 corpora and lexical resources.
"""

summary = summarize_text_no_nltk(text, num_sentences=2)
print("Summary:\n", summary)
