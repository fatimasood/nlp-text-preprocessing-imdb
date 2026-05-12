# 🧠 NLP Text Preprocessing Using Real-World Data

## IMDb Movie Reviews — Complete Preprocessing Pipeline

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![NLTK](https://img.shields.io/badge/NLTK-3.8-green.svg)](https://www.nltk.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3-orange.svg)](https://scikit-learn.org/)
[![Colab](https://img.shields.io/badge/Open_in-Colab-orange.svg)](https://colab.research.google.com/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-blue.svg)](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

---

## 📌 Project Overview

This project presents a **complete NLP text preprocessing pipeline**. The pipeline is applied to a real-world dataset — the **IMDb 50K Movie Reviews** from Kaggle.

Raw text from the internet is messy. It contains HTML tags, emojis, contractions, typos, mixed case, URLs, and inconsistent punctuation. Machine learning models cannot understand such noise directly. Text preprocessing cleans and standardizes this raw data into a format that NLP algorithms can process effectively.

### 🎯 What This Project Covers

- ✅ Loading and exploring a **real-world Kaggle dataset** (50,000 reviews)
- ✅ Implementing **8 preprocessing techniques** with detailed explanations
- ✅ **Comparing Stemming vs Lemmatization** using actual IMDb review words
- ✅ Measuring **vocabulary reduction** (47.6% achieved)
- ✅ Validating preprocessing impact with **sentiment classification** (0.48% improvement)
- ✅ **Critical analysis** of each technique — what works, what fails, and why
- ✅ Complete **Google Colab notebook** with all code and outputs

---

## 📊 Dataset Information

### Source
🔗 **Kaggle Link:** [IMDb Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

### Dataset Statistics

| Property | Value |
|:---|:---|
| **Dataset Name** | IMDb Dataset of 50K Movie Reviews |
| **Total Reviews** | 50,000 |
| **Positive Reviews** | 25,000 (50%) |
| **Negative Reviews** | 25,000 (50%) |
| **Features** | `review` (text), `sentiment` (label) |
| **Average Review Length** | 233 words |
| **Shortest Review** | 4 words |
| **Longest Review** | 2,523 words |
| **Reviews Containing HTML Tags** | 42,371 (84.7%) |
| **Reviews Containing Emojis** | ~1,500 (3%) |
| **Language** | English |
| **Domain** | Movie Reviews (User-Generated Web Content) |
| **License** | Open for Research and Educational Use |

### Why I Chose This Dataset

1. **Real-world noise** — HTML tags from web scraping, emojis, typos, contractions, excessive punctuation
2. **84.7% reviews have HTML `<br>` tags** — thoroughly tests the HTML removal step
3. **Balanced classes** — 25,000 positive + 25,000 negative = no class imbalance
4. **Benchmark dataset** — widely used in NLP research papers
5. **Large enough** — 50,000 reviews show statistically meaningful preprocessing impact
6. **Free and accessible** — anyone can download from Kaggle

### Sample Raw Reviews

**Positive Review:**
> One of the other reviewers has mentioned that after watching just 1 Oz episode you'll be hooked. They are right, as this is exactly what happened with me.\<br />\<br />The first thing that struck me about Oz is its brutality and unflinching scenes of violence...

**Negative Review:**
> A wonderful little production. \<br />\<br />The filming technique is very unassuming- very old-time-BBC fashion and gives a comforting, and sometimes discomforting, sense of realism to the entire piece...

**Notice the issues:** `<br />` HTML tags, contractions ("you'll"), hyphenated phrases, informal expressions. All these need preprocessing.

---

## 📈 Key Results

Accuracy with RAW text:    0.8350
Accuracy with PROCESSED text: 0.8390
Improvement: 0.48%


> Lemmatization preserves real words — better for NLP tasks.

