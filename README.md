# NFL_2026_Pass_Analytics_and_Prediction

This project explores whether an NFL pass play can be predicted as successful **before the outcome occurs**, using player-level tracking data and play-level contextual information. The goal is to demonstrate how **spatiotemporal data**, feature engineering, and machine learning can be combined to model real-world, event-based outcomes.

## 🏈 Problem Statement

Passing plays are influenced by multiple dynamic factors such as player positioning, movement speed, defensive pressure, and game context. This project frames pass outcome prediction as a **binary classification problem**, aiming to estimate the likelihood of a completed pass using information available during the play.

## 📊 Data & Features

The analysis uses NFL player tracking and play data to engineer features including:

* Player speed and movement dynamics
* Distances between offensive and defensive players
* Defensive proximity and pressure indicators
* Play-level and game-state contextual variables

Careful preprocessing and **group-aware train/test splitting** were applied to prevent play-level data leakage.

## 🤖 Modeling Approach

* Performed exploratory data analysis (EDA) to understand relationships between spatial, temporal, and contextual variables
* Trained and evaluated **Random Forest**, **Logistic Regression** and **Gradient Boosting** models
* Compared model performance using **accuracy, F1 score, and precision-recall metrics**
* Analyzed model behavior to identify key drivers of pass success

## 📈 Results & Insights

The models demonstrate that combining spatiotemporal tracking data with contextual features significantly improves pass success prediction. Defensive positioning, offensive spacing, and situational context emerged as strong predictors of play outcome. Overall prediction rate was 72.51%

## 🛠️ Tech Stack

* **Languages:** Python
* **Libraries:** Pandas, NumPy, scikit-learn, Matplotlib
* **Techniques:** Feature Engineering, Classification Models, Model Evaluation, EDA

## 🚀 Future Improvements

* Model interpretability using SHAP or feature importance analysis
* Usage of Geometric GNNs for better understanding of spatiotemporal data
* Probability calibration for improved decision-making
* Extension to real-time or in-play prediction scenarios
