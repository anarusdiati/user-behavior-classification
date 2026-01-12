# User Behavior Classification
Predict whether a user session will result in a conversion based on behavioral signals. 

This project focuses on predicting user purchase intent based on behavioral signals collected during online shopping sessions. The goal is to demonstrate how machine learning can support user-centric product decisions while maintaining a privacy-conscious approach.

<h2>Problem Statement</h2>
Understanding user intent early allows digital products to improve user experience without relying on intrusive personal data.



<h2>ML Task</h2>

- Supervised Learning
- Binary Classification

<h2>Business Relevance</h2>
Early prediction of user intent enables better UX personalization and decision-making without intrusive data collection.

<h2>Dataset</h2>

Online Shoppers Purchasing Intention Dataset ([UCI](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset) / [Kaggle](https://www.kaggle.com/datasets/henrysue/online-shoppers-intention))

**Dataset Characteristics**
- Type: Multivariate dataset
- Subject Area: Business/E-commerce
- Associated Tasks: Classification, Clustering

**Data Quality**</br>
No missing values, clean dataset

**Feature Set**</br>
Total Features: 18 attributes (17 features + 1 target)

**Numerical Features (10)**
- Administrative: Count of administrative pages visited
- Administrative_Duration: Time spent on administrative pages
- Informational: Count of informational pages visited
- Informational_Duration: Time spent on informational pages
- ProductRelated: Count of product-related pages visited
- ProductRelated_Duration: Time spent on product-related pages
- BounceRates: ercentage of visitors who enter and leave without interaction
- ExitRates: Percentage of pageviews that were the last in the session
- PageValues: Average value for web pages before completing e-commerce transaction
- SpecialDay: Closeness to special days

**Categorical Features (8)**
- Operating System: Visitor's operating system
- Browser: Web browser used
- Region: Geographical region of visitor
- Traffic Type: Traffic source type
- Visitor Type: New or returning visitor
- Weekend: Weekend visit indicator
- Month: Month of session occurrence

**Target Variable**
Revenue (session outcome indicator)
- True: Session ended with shopping transaction
- False: Session did not end with shopping transaction

**Class Distribution**
- Total Sessions: 12,330
- Negative Class (No Purchase): 10,422 sessions (84.5%)
- Positive Class (Purchase): 1,908 sessions (15.5%)
- Class Imbalance Ratio: 5.46:1 (Imbalanced dataset)


<h2>Methodology</h2>

- Logistic Regression (as baseline)
- Random Forest
- XGBoost / LightGBM
- SHAP (for interpretability)

<h2>Metrics for Evaluation</h2>

- ROC-AUC (utama)
- Precision / Recall
- Confusion Matrix

<h2>Tech Stack</h2>

- Python
- Scikit-learn
- XGBoost
- SHAP
- Google Colab

<h2>Key Insights</h2>

<h2>Limitations & Future Works</h2>

<h2>Medium</h2>

Read this project article on my [Medium](https://medium.com/@anarusdiati)
