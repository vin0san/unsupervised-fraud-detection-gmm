# Unsupervised Fraud Detection with GMM

> **0.93 ROC-AUC · 280,000+ transactions · Zero labeled training data**

Anomaly detection on financial data using Gaussian Mixture Models and Bayes posterior scoring.
Simulates the real-world constraint where fraud labels are unavailable at training time.

## Steps
- Load Kaggle Credit Card Fraud dataset (link below).
- Drop labels to simulate an unsupervised scenario.
- Fit GMM, compute log-likelihood and anomaly scores.
- Flag top N% transactions as potential fraud.
- Evaluate against true labels (precision, recall, ROC-AUC).

Dataset: [Credit Card Fraud Detection on Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

## Files
- `fraud_detection_gmm.ipynb`: Jupyter notebook with code + markdown explanations.
- `README.md`: This file.

## How to run
1. Download `creditcard.csv` from Kaggle and place it in the same folder.
2. Open the notebook in Jupyter/Colab and run all cells.

## Results
At 2% flagging threshold: Recall ≈ 71%, ROC-AUC ≈ 0.93.

## License
[MIT](LICENSE)
