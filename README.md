# 🏀 Basketball DNA (BNA) Project: ML Analysis for Optimal Position Prediction

Korean version REAME is [here](./README.ko.md).

> **[Academic Project]** This machine learning project was developed as part of a university course to analyze and predict optimal basketball positions based on player data.

## 🌟 Project Overview

The **BNA (Basketball DNA) Project** aims to **predict the most suitable basketball position (PG, SG, SF, PF, C)** for NBA players by leveraging their game statistics and physical information (height, weight). The project also explores the practical limitations inherent in position classification in basketball.

## 🛠️ Tech Stack and Methodology

| Category | Description |
| :--- | :--- |
| **Objective** | Classification of 5 distinct positions based on a player's **physical attributes and game statistics**. |
| **Data Source** | NBA Player Data from Kaggle (1996–2024 seasons). |
| **Preprocessing**| Outlier removal using the MAD method, followed by extensive **Feature Engineering** (e.g., BMI, 3-Point Attempt Rate, Per-Minute Metrics). |
| **Primary Models**| Logistic Regression, Random Forest Classifier. |
| **Language/Libraries** | `Python`, `Pandas`, `NumPy`, `Scikit-learn`, `Matplotlib`, `Seaborn` |

## 💡 Final Insight

The model's 5-position classification accuracy stalled at **74% $\sim$ 76%**. This stagnation was not primarily due to limitations in the machine learning algorithms, but rather the **domain characteristic** of modern basketball where **positional boundaries are increasingly blurred**.

* **The Critical Role of Domain Knowledge:** Misclassifications predominantly occurred between position pairs with ambiguous roles in real life (e.g., PF/C and PG/SG). To address this, **domain knowledge** was applied to simplify the target into three categories: **G (Guard), F (Forward), and B (Big)**. This simplification resulted in a sharp accuracy increase to **$\approx 87\%$**.
* **Conclusion:** This project confirms the paramount importance of not just complex algorithms or large datasets, but of **deeply understanding the domain's specific characteristics and incorporating that real-world knowledge into the modeling process** to optimize machine learning performance.

