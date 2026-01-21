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

Online Shoppers Purchasing Intention Dataset ( [UCI](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset) / [Kaggle](https://www.kaggle.com/datasets/henrysue/online-shoppers-intention) )

**Dataset Characteristics**
- Type: multivariate dataset
- Subject area: business/e-commerce
- Associatedtasks: classification, clustering

**Data Quality**</br>
No missing values, clean dataset

**Feature Set**</br>
Total features: 18 attributes (17 features + 1 target)

**Numerical Features (10)**
- Administrative: count of administrative pages visited
- Administrative_Duration: time spent on administrative pages
- Informational: count of informational pages visited
- Informational_Duration: time spent on informational pages
- ProductRelated: count of product-related pages visited
- ProductRelated_Duration: time spent on product-related pages
- BounceRates: percentage of visitors who enter and leave without interaction
- ExitRates: percentage of pageviews that were the last in the session
- PageValues: average value for web pages before completing e-commerce transaction
- SpecialDay: closeness to special days

**Categorical Features (8)**
- Operating System: visitor's operating system
- Browser: web browser used
- Region: geographical region of visitor
- Traffic Type: traffic source type
- Visitor Type: new or returning visitor
- Weekend: weekend visit indicator
- Month: month of session occurrence

**Target Variable**
Revenue (session outcome indicator)
- True: session ended with shopping transaction
- False: session did not end with shopping transaction

**Class Distribution**
- Total sessions: 12,330 sessions
- Negative class (no purchase): 10,422 sessions (84.5%)
- Positive class (purchase): 1,908 sessions (15.5%)
- Class imbalance ratio: 5.46:1 (imbalanced dataset)


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
- Kaggle
- GitHub

<h2>Key Insights</h2>

<h2>Limitations & Future Works</h2>

<h2>Medium</h2>

Read this project article on my [Medium](https://medium.com/@anarusdiati)
