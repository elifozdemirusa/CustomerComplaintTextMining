# Customer Complaint Text Mining

An end-to-end Natural Language Processing (NLP) and machine learning project for analyzing customer complaint text data using both supervised and unsupervised learning techniques.

This project demonstrates how unstructured text data can be transformed into actionable business insights through classification, clustering, and topic modeling.

---

##  Project Overview

Customer complaint data contains valuable signals about customer pain points, service quality, and operational risks.  
In this project, we analyze consumer complaint narratives to:

- Automatically classify complaints into product categories
- Discover hidden themes and patterns without predefined labels
- Compare multiple machine learning models using a unified evaluation framework

The project was developed as part of the **M.S. in Business Analytics** program at **Western New England University**.

---

##  Dataset

- **Source:** Consumer Financial Protection Bureau (CFPB)
- **File used:** `data/complaints_sample.csv`
- **Data type:** Text-based consumer complaint narratives
- **Key column:** `Consumer complaint narrative`

A reduced sample dataset is included in this repository to ensure reproducibility and easy execution.

---

##  Data Preparation

The dataset was cleaned and prepared using the following steps:

- Removal of irrelevant columns
- Deduplication of complaint records
- Removal of missing complaint narratives
- Filtering to top 5 most frequent product categories
- Class balancing for fair supervised model comparison

---

##  Machine Learning Models

###  Supervised Learning (Classification)
A unified “horse race” framework was used so all models were trained and tested on the **exact same data split**.

Models evaluated:
- **Random Forest + Bag-of-Words**
- **Logistic Regression + TF-IDF**
- **Naive Bayes + TF-IDF**

**Evaluation Metric:** Accuracy  
**Additional Analysis:** Confusion Matrix & Classification Report

---

###  Unsupervised Learning (Pattern Discovery)

To uncover hidden structures in complaint text:

- **K-Means Clustering** (TF-IDF features)
  - Evaluated using **Silhouette Score**
- **Latent Dirichlet Allocation (LDA)**
  - Topic modeling evaluated via **Perplexity**

These models provide insights into complaint themes without relying on labeled data.

---

##  Results Summary

- Random Forest and Logistic Regression achieved approximately **80% classification accuracy**
- K-Means successfully grouped complaints into interpretable clusters
- LDA revealed meaningful complaint topics such as:
  - Credit reporting issues
  - Bank fees and account problems
  - Debt collection practices
  - Mortgage payment disputes

---

##  Business Value

This project demonstrates how NLP can be used to:

- Automate complaint routing and categorization
- Identify systemic issues across large volumes of text data
- Support customer service, compliance, and risk management teams
- Reduce manual review costs while improving response speed

---

## How to Run Locally

1. **Clone the repository:**
```bash
git clone https://github.com/elifozdemirusa/CustomerComplaintTextMining.git
```
2. **Navigate to the project directory**
```bash
cd CustomerComplaintTextMining
```
3.**Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
4.**Launch Jupyter Notebook**
```bash
jupyter notebook notebooks/complaints_text_mining.ipynb
```



