Leakage-Controlled Machine Learning for Geriatric Functional-Dentition Prediction

This repository contains the complete analysis code for the paper:

"Leakage-Controlled Machine Learning for Geriatric Functional-Dentition Prediction" Submitted to IEEE Access, 2026.

Overview

We benchmark seven classifiers (Logistic Regression, Random Forest, Extra-Trees, Histogram Gradient Boosting, XGBoost, LightGBM, CatBoost) for three-class functional-dentition prediction on the Harvard Dataverse Geriatric Oral Health Determinants cohort (N=421, 96 variables). A formal target-leakage audit reveals that clinical tooth-pair counts near-deterministically restate the label, inflating macro F1 from 0.40 to 0.81. Under a leak-free protocol, no gradient-boosting model significantly outperforms Logistic Regression, and psychosocial features (AAQ, OHIP-14) provide the largest legitimate predictive gain.

Repository Contents
File	Description
complete_notebook.ipynb	Full analysis pipeline: data loading, leakage audit, Experiments A and B, statistical comparison, ablation, calibration, and all figures/tables
dataset.csv	Geriatric Oral Health Determinants dataset (also available from Harvard Dataverse)
Dataset

The dataset is publicly available from the Harvard Dataverse under the Geriatric Oral Health Determinants project.

Requirements
Python 3.8+
scikit-learn, XGBoost, LightGBM, CatBoost
pandas, numpy, matplotlib, seaborn, scipy
Citation

If you use this code, please cite our paper (citation details will be added upon publication).

License

This project is provided for academic and research purposes.
