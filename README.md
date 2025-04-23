# Challengers

Predicting ATP tennis match outcomes with machine‑learning models so we (responsibly!) improve our odds when placing wagers.

---

## Table of Contents
1. [Project Motivation](#project-motivation)
2. [Dataset](#dataset)
3. [Problem Statement](#problem-statement)
4. [Methods & Techniques](#methods--techniques)
5. [Project Plan](#project-plan)
6. [Getting Started](#getting-started)
7. [Team](#team)
8. [Inspiration](#inspiration)

---

## Project Motivation
We enjoy betting on tennis but admit we are *awful* at picking winners. By building the most accurate predictive model we can, we hope to gain a data‑driven edge over gut feelings.

## Dataset
- **Source:** [Jeff Sackmann’s ATP match repository](https://github.com/JeffSackmann/tennis_atp)
- **Data types:** Categorical & quantitative match‑level records dating back to 1968.
- **Key features under consideration:**
  - Current ATP ranking of each player (pure skill indicator)
  - Career earnings & seasonal prize money
  - Historical win/loss counts
  - Game & set score differentials
- **NOTE:** You’ll need to make sure the years 2018‑2024 are in the directory named `tennis_atp/...`, or just clone the repo in the same folder.

## Problem Statement
*Can we accurately classify the winner of an upcoming tennis match using historical performance data?* Success will be measured by overall accuracy and betting unit return on an unseen 2025 test set.

## Methods & Techniques
This is a supervised **classification** task.  We will experiment with:
- Logistic Regression
- K‑Nearest Neighbors (KNN)
- Decision Trees & Random Forests
- Gradient Boosting (e.g. XGBoost, AdaBoost)
- Regularized models (L1/L2)

For each algorithm we will perform hyper‑parameter tuning (grid/random search) and apply ensemble techniques such as bagging and boosting where applicable.

## Project Plan
1. **Data Cleaning & Pre‑processing**  
   ‑ Deduplicate matches, handle missing values, encode categoricals, remove or combine highly collinear variables.
2. **Exploratory Data Analysis**  
   ‑ Summary stats & visualizations to understand distributions and relationships.
3. **Model Training**  
   ‑ Train baseline models, evaluate with cross‑validation, iterate on feature engineering.
4. **Hyper‑parameter Tuning**  
   ‑ Optimize promising models; evaluate on a 2024 hold‑out set.
5. **Final Evaluation**  
   ‑ Test on 2025 matches and compare to the 83 % accuracy benchmark.
6. **Deployment (Stretch Goal)**  
   ‑ Package the best model into a CLI or web app for real‑time predictions.

## How Is It Run?
We use Jupyter Notebook to run this so just open the Challengers.ipynb through the notebook and run.

## Team
| Role           | Member                     |
|----------------|----------------------------|
| **Leader**     | Anton Salvador             |
| Data Engineers | Mathew Alangadan • Ryder Keeney |
| ML Engineers   | Dylan Tallon • Zachary Miguel Allarey |

## Inspiration
A video by *AlgoBeans* ("Building a Tennis Match Predictor – 83 % Accuracy", 2025) demonstrated an 83 % Random Forest model on 2025 data. We aim to beat that score and share our improvements.

---

> **Disclaimer:** This project is for educational purposes only. Gamble responsibly.


