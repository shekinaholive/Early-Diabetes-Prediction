# Early Diabetes Prediction — MLP, XGBoost and TabNet

A comparative machine-learning project using structured health data to explore **diabetes classification** and feature-based interpretability.

## Overview

The experiment compares:

- **MLP:** Neural-network baseline
- **XGBoost:** Gradient-boosted decision trees
- **TabNet:** Attention-based deep learning for tabular data

The work includes exploratory data analysis, preprocessing, handling missing values, class-imbalance treatment using **SMOTE**, and comparison of model predictions.

## Reported results

| Model | Project-reported accuracy |
| --- | ---: |
| MLP | 75% |
| XGBoost | 79% |
| TabNet | **80%** |

These figures come from the project's previous README and resume. They have **not been re-executed** for this documentation update. The repository does not currently provide a separate, verified machine-readable experiment report for independent comparison.

## Repository contents

- **AA_AML_ (1).ipynb** — project notebook (check that it opens and runs in your chosen notebook environment)
- **README.md** — project overview and reporting notes

## How to reproduce

1. Obtain the original tabular dataset used for the experiments. The prior README refers to **diabetes.csv**, but the dataset is not provided at the repository root.
2. Install the libraries used by the notebook; depending on the experiment, these include **numpy**, **pandas**, **scikit-learn**, **xgboost**, **torch**, **pytorch-tabnet** and plotting libraries.
3. Open the notebook, update any input paths and run the experiment in order.
4. Verify dataset partitions and apply imputation/scaling/SMOTE **only on training data** to avoid data leakage, then recalculate evaluation metrics.

## Limitations and next steps

- Document the dataset origin, license, class prevalence and exact train/test split.
- Report recall, precision, F1-score, ROC-AUC and calibration alongside accuracy.
- Add repeatable evaluation scripts and environment versions.
- TabNet feature attributions are model explanations, **not causal medical findings**.

## Intended use

**Academic experiment only.** Not suitable for medical screening, diagnosis or treatment decisions.

---
**Author:** [Shekinah Olive](https://github.com/shekinaholive)
