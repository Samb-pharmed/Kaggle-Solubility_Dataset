# Kaggle-Solubility_Dataset
Machine learning project using AqSolDB to predict aqueous solubility from molecular descriptors. Includes EDA, baseline and ensemble model comparison, Extra Trees selection as best model, and prediction examples for new molecules to support early pharmaceutical preformulation screening.

# AqSolDB Aqueous Solubility Prediction

**Author:** Samb-pharmed  
**Dataset:** AqSolDB: A curated aqueous solubility dataset [Kaggle](https://www.kaggle.com/datasets/sorkun/aqsoldb-a-curated-aqueous-solubility-dataset)  
**Project type:** Applied machine learning for pharmaceutical preformulation

## Project Overview

This project uses the AqSolDB dataset to predict aqueous solubility from molecular descriptors. The aim is to explore whether machine learning can support early pharmaceutical preformulation by identifying compounds with potential solubility risks before experimental testing.

## Repository Structure

- `AqSolDB- Sec 1- EDA, RF and GB models.ipynb`  
  Data inspection, exploratory data analysis, baseline modelling, Random Forest, and Gradient Boosting.

- `AqSolDB- Sec 2- more models.ipynb`  
  Additional model benchmarking including Extra Trees, LightGBM, XGBoost, SVR, Elastic Net, and PLS.

- `AqSolDB- Sec 3- Test 5 new molecule with Extra Trees.ipynb`  
  Uses the best-performing model to predict solubility for five external example molecules.

## Methods

The workflow included:

- Data inspection and quality assessment
- Exploratory data analysis
- Correlation analysis
- Baseline modelling
- Model comparison using MAE, RMSE, and R²
- Feature importance analysis
- External prediction examples

## Models Compared

- Mean Baseline
- Linear Regression
- Random Forest
- Gradient Boosting
- Extra Trees
- LightGBM
- XGBoost
- Support Vector Regression
- Elastic Net
- Partial Least Squares

## Key Result

Extra Trees was the best-performing model:

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Extra Trees | 0.720 | 1.059 | 0.793 |

## Pharma Relevance

This type of model can support early preformulation decision-making by estimating aqueous solubility risk from molecular descriptors. It may help prioritise compounds for experimental testing and identify candidates that may require solubility-enhancing formulation strategies.

## Limitations

The model should be used as a decision-support tool, not as a replacement for experimental solubility testing. It does not directly account for pH-dependent ionisation, salt form, polymorphism, particle size, crystal form, or experimental method variability.

## Dataset Source

The dataset is available on Kaggle:  
[AqSolDB: A curated aqueous solubility dataset](https://www.kaggle.com/datasets/sorkun/aqsoldb-a-curated-aqueous-solubility-dataset)

## Author

Developed by **Samb-pharmed** as part of applied data science practice in pharmaceutical R&D and preformulation.
