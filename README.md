# Predictive Maintenance Using Machine Learning

## Overview
This project uses the AI4I 2020 Predictive Maintenance dataset to predict machine failures from operating measurements using machine learning.

## Objectives
- Explore and preprocess machine sensor data.
- Compare Decision Tree, Random Forest, and Logistic Regression classifiers.
- Address class imbalance and evaluate models using precision, recall, and F1-score.
- Investigate classification-threshold tuning to balance missed failures and false alarms.
- Examine feature importance to identify influential model inputs.

## Dataset
AI4I 2020 Predictive Maintenance Dataset, available on Kaggle.

The dataset contains 10,000 records with machine operating measurements and failure labels.
Source: [AI4I 2020 Predictive Maintenance Dataset — Kaggle](https://www.kaggle.com/datasets/stephanmatzka/predictive-maintenance-dataset-ai4i-2020)

## Methods and Tools
- Python, Pandas
- scikit-learn
- Google Colab
- Classification metrics and feature-importance analysis

## Final Model Results
The selected Random Forest model, using a classification threshold of 0.60, achieved these test-set results:

- **Accuracy:** 97.65%
- **Failure precision:** 63.3%
- **Failure recall:** 73.5%
- **Failure F1-score:** 68.0%
- **Failures detected:** 50 out of 68
- **Missed failures:** 18
- **False alarms:** 29

## Key Findings
Torque, rotational speed, and tool wear were the three most influential features according to the model's feature-importance scores.

## Limitations
This project uses a public benchmark dataset rather than live industrial sensor data. Results do not establish performance on real equipment. The test set was inspected during earlier model comparisons, so the final evaluation is not a completely untouched assessment.

## Future Improvements
- Validate the model on independent or real-world data.
- Explore additional models and systematic hyperparameter tuning.
- Investigate precision-recall trade-offs and model interpretability.

## Disclaimer
This is an educational machine-learning project, not a deployed industrial predictive-maintenance system.
