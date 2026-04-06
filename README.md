# An Empirical Comparison of Supervised Learning Algorithms

This repository contains a comparative study of three fundamental machine learning algorithms—**Logistic Regression, Decision Trees, and Random Forests**—evaluated across three distinct UCI datasets. 

The project investigates how model performance scales with varying training data partitions (20%, 50%, and 80%) to simulate different data-availability scenarios.

## Datasets Used
We utilized the following datasets from the UCI Machine Learning Repository:
1. **Breast Cancer Wisconsin (Diagnostic):** Numerical features for binary classification (Malignant/Benign).
2. **Adult Income:** High-dimensional categorical and numerical data to predict if income exceeds $50K/year.
3. **Mushroom:** Categorical features used to identify poisonous vs. edible mushrooms.

## Methodology
The analysis follows a standardized pipeline:
* **Preprocessing:** Automatic fetching via `ucimlrepo`, handling missing values, and one-hot encoding categorical variables.
* **Algorithm Suite:** * **Logistic Regression:** A parametric linear model.
    * **Decision Tree:** A non-parametric tree-based model.
    * **Random Forest:** An ensemble method to reduce variance and overfitting.
* **Evaluation:** Models were tested across different training sizes to observe the impact of data volume on accuracy and generalization.

## Key Findings
* **Ensemble Superiority:** Random Forest generally outperformed single Decision Trees, particularly on the complex **Adult** dataset, by maintaining a smaller generalization gap.
* **Linear Separability:** Logistic Regression performed exceptionally well on the **Breast Cancer** dataset (97.4% accuracy), suggesting that the boundary between classes in that feature space is largely linear.
* **Data Volume:** Across all models and datasets, increasing the training partition from 20% to 80% resulted in significant gains in predictive reliability.

## Getting Started
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/supervised-learning-benchmarks.git](https://github.com/YOUR_USERNAME/supervised-learning-benchmarks.git)
