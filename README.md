# Online Shoppers Purchase Intention Analysis

<h2>Overview</h2>

This project explores how user behavior on an e-commerce website translates into purchase decisions. Using the Online Shoppers Intention Dataset from the UCI Machine Learning Repository, the goal is not only to build a predictive model, but also to understand why users convert, and how these insights can be translated into meaningful business actions. The project follows an end-to-end data science workflow, from exploratory analysis to model interpretability using SHAP, with a strong emphasis on clarity, reasoning, and decision-making rather than just model accuracy.

<h2>Problem Statement</h2>

E-commerce platforms collect large amounts of behavioral data, but raw data alone does not answer the most important question:

**What truly drives users to make a purchase?**

This project aims to:
- Predict whether a website session will result in a purchase.
- Identify the most influential behavioral and temporal factors.
- Translate model outputs into actionable business insights.

<h2>Dataset</h2>

- Name: Online Shoppers Purchasing Intention Dataset ( [UCI](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset) / [Kaggle](https://www.kaggle.com/datasets/henrysue/online-shoppers-intention) )
- Samples: 12,330 sessions
- Target Variable: `Revenue` (binary: purchase or no purchase)

The dataset contains a mix of numerical, categorical, and behavioral features such as page durations, visit types, and timing information.

<h2>Project Structure</h2>

The project is structured into four main stages to ensure clarity and reproducibility.

<h3>1. Exploratory Data Analysis</h3>

At this stage, the dataset is explored to understand:

- Overall data structure and feature types
- Class distribution of the target variable
- Behavioral patterns between converting and non-converting users

This step helps validate assumptions and guides downstream preprocessing and modeling choices.

<h3>2. Data Preprocessing and Feature Engineering</h3>

The preprocessing pipeline includes:
- Separating features and target
- Encoding categorical variables
- Train-test split with stratification
- Feature scaling for numerical stability
- Handling class imbalance using resampling techniques
- Building a unified preprocessing pipeline to avoid data leakage

At the end of this step, the data is fully model-ready and consistent across experiments.

<h3>3. Modeling and Baseline Comparison</h3>

Multiple models are trained and compared to balance performance and interpretability:

- Logistic Regression as a baseline
- Random Forest for non-linear feature interactions
- XGBoost for optimized gradient boosting performance

Evaluation focuses on metrics suitable for imbalanced classification, such as precision, recall, and F1-score, rather than accuracy alone.

<h3>4. Model Evaluation and Interpretability</h3>

The best-performing model is evaluated using:
- Confusion matrix
- Classification report
- Precision-recall trade-off analysis

To move beyond black-box predictions, **SHAP** (SHapley Additive exPlanations) is used to:

- Identify global feature importance
- Understand how individual features contribute to predictions
- Extract key business insights from model behavior

This step bridges the gap between machine learning and real-world decision-making.

<h2>Key Insights</h2>

Several consistent patterns emerge from the analysis:

- Longer interaction time with product-related pages significantly increases purchase probability.
- Returning visitors are far more likely to convert than new users.
- Temporal factors such as month and weekend visits influence buying behavior.

These insights highlight opportunities for personalization, remarketing, and timing-based campaign strategies.

<h2>Tech Stack</h2>

- Python
- Pandas, NumPy
- Matplotlib & Seaborn
- Scikit-learn
- XGBoost
- SHAP

<h2>Limitations and Future Work</h2>

While the results are promising, several improvements are possible:

- Hyperparameter optimization for advanced models
- Deeper session-level or sequential behavior analysis
- Integration with real-time or streaming data
- Deployment as a lightweight decision-support system

<h2>Final Notes</h2>

This project emphasizes thinking before modeling, and understanding before optimizing. The goal is not just to predict conversions, but to explain them in a way that humans, businesses, and product teams can act upon.

<h2>Medium</h2>

Read this project article on my [Medium]([https://medium.com/@anarusdiati](https://medium.com/@anarusdiati/predicting-purchase-intention-from-online-user-behavior-56caa07e9e44))

Let's connect
