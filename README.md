# ML Final Project: E-Commerce Purchase Intent Prediction

This repository contains my **Machine Learning final project** (CSC-321: Data Mining & Machine Learning), where I analyze the **UCI Online Shoppers Purchasing Intention** dataset to predict whether a browsing session ends in a purchase (`Revenue`).

## Project Highlights
- **End-to-end ML workflow** in a reproducible notebook (data loading → EDA → feature engineering → training → evaluation → conclusions)
- **Exploratory Data Analysis (EDA):** class imbalance, distributions, correlation analysis, and buyer vs non-buyer comparisons using histograms, box plots, and scatter plots
- **Feature engineering:** `Total_Duration`, `Total_Pages`, `Has_PageValue`, `IsSpecial`, and calendar interaction features like `Month_Weekend`
- **Imbalance handling:** compared **original vs oversampled vs undersampled** training sets
- **Models:** ZeroR baseline, **Logistic Regression**, **k-NN**, and **Gaussian Naive Bayes**
- **Evaluation metrics:** accuracy, precision, recall, plus **MAE/RMSE** computed on predicted probabilities
- **Interpretability:** Logistic Regression coefficient analysis to identify the strongest drivers of purchase intent
- **Behavioral insight:** “near-miss” non-buyers analysis (sessions predicted as likely to purchase but did not)

## Key Findings (High-Level)
- Buyer sessions tend to show **higher engagement** (more pages, longer durations), **higher PageValues**, and **lower bounce/exit behavior** than non-buyers.
- Class balancing increases **recall** for buyers but can reduce overall accuracy and increase probability error, showing a clear trade-off depending on the goal.

## Dataset
- **Source:** UCI Machine Learning Repository — Online Shoppers Purchasing Intention  
- **Size:** 12,330 sessions, 17 features + target (`Revenue`)  
- **Task:** Binary classification (purchase vs no purchase)

## How to Run
1. Open the notebook in **Google Colab** (recommended) or Jupyter.
2. Install dependencies (the notebook includes install cells when needed).
3. Run all cells top-to-bottom.
4. If using a local CSV, place `online_shoppers_intention.csv` next to the notebook.  
   Otherwise, use the UCI loader option in the notebook for full reproducibility.

## Repository Structure
- `notebook.ipynb` — main research notebook (write-up + code)
- `README.md` — project overview (this file)

## Skills & Tools
Python, Pandas, NumPy, scikit-learn, imbalanced-learn, Matplotlib, Seaborn, feature engineering, classification, model evaluation, interpretability, imbalanced learning.

---
If you have questions or want to discuss the approach, feel free to reach out!
