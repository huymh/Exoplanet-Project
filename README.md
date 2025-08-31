# 💫 Exoplanet Exploaratory Data Analysis and Classification with Machine Learning

## 📰 Overview
This project analyzes NASA’s Kepler exoplanet dataset to classify exoplanets as Confirmed, Candidate, or False Positive. The workflow includes exploratory data analysis (EDA) to understand feature distributions and correlations, data preprocessing including encoding and scaling, feature selection, and comparison of multiple machine learning models to identify the most effective classifiers.

## 💡 Insights
Here is a preview of some of the questions explored within this dataset. Full analysis and model evaluation are available in the Jupyter Notebook.

Exploratory Data Analysis
- What are the key features that differentiate confirmed exoplanets from false positives?
- How are various exoplanet parameters (e.g., radius, orbital period, stellar flux) distributed across classes?
- Are there correlations among planetary and stellar features that can inform classification?

Model Evaluation
- How do models like Random Forest, XGBoost, LightGBM, Gradient Boosting, and MLP Neural Networks compare in predicting exoplanet classes?
- Which model achieves the best performance on metrics such as accuracy and weighted F1 score?
- How does feature selection impact model performance?

## 📊 Data
[NASA's Kepler Exoplanet Candidate Dataset](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=cumulative) and [column descriptions](https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html)

## 🛠 Tools Used
- Jupyter Lab / Jupyter Notebook : Python
- Libraries : numpy, pandas, matplotlib, seaborn, scikit-learn, xgboost, lightgbm
