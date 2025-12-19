# CustomerComplaintTextMining
NLP and machine learning project for analyzing customer complaint text data using supervised and unsupervised models.
## Overview
This project demonstrates an end-to-end **NLP and Machine Learning pipeline**
for analyzing real-world customer complaint text data.

It covers:
- Text preprocessing and feature engineering
- Supervised classification with a unified evaluation framework
- Unsupervised learning for pattern discovery
- Business interpretation of model outputs

The project emphasizes **fair model comparison**, **interpretability**, and
**practical business insights**, not just accuracy scores.
## Machine Learning & NLP Techniques

**Supervised Learning**
- Random Forest (Bag-of-Words)
- Logistic Regression (TF-IDF)
- Multinomial Naive Bayes
- Unified train/test split ("horse race" comparison)
- Accuracy, classification report, confusion matrix

**Unsupervised Learning**
- K-Means clustering with silhouette score evaluation
- LDA topic modeling with perplexity-based scoring
- Manual cluster and topic interpretation

**Text Processing**
- TF-IDF and Bag-of-Words vectorization
- N-grams (unigrams & bigrams)
- Stopword removal and frequency filtering

## Business Value

This system can support financial institutions by:

- Automatically categorizing customer complaints (~80% accuracy)
- Reducing manual review workload for support teams
- Identifying emerging complaint patterns through unsupervised learning
- Improving response prioritization for high-risk complaint categories

The combination of supervised and unsupervised methods provides both
**automation** and **insight discovery**.

## Dataset

The original CFPB consumer complaint dataset contains millions of records and
cannot be fully included in this repository.

For reproducibility and efficiency, this project uses a **cleaned sample
dataset**:

- `data/complaints_sample.csv`

The sample preserves the original structure and is sufficient to reproduce
all analyses, models, and visualizations in this project.

## How to Run

1. Clone the repository
2. Install required libraries
3. Run the main analysis notebook

```bash
python src/main.py


