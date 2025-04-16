# DML_RF

This repository contains a clean and minimal Python implementation of **Double Machine Learning (DML)** using **Random Forest** . 
The script performs causal inference by estimating the **Average Treatment Effect (ATE)** through three different methods and visualizing 
the bias. 

- **Ordinary Least Squares (OLS)**: Baseline estimation without controlling for selection bias.  
- **Naive DML**: Splits the sample into two parts — one for estimating nuisance parameters, the other for estimating the ATE.  
- **Cross-Fitting DML**: Splits the sample into two and alternates roles between folds to estimate nuisance parameters and ATE, reducing overfitting and bias.

The goal is to compare the effectiveness of these methods with visualized plot

## Key Features

- 🔍 Compares **OLS**, **naive DML**, and **cross-fitting DML**
- 🌲 Uses **Random Forest** to model nuisance components
- 🧪 Easy-to-modify structure with real world data
- 📉 Demonstrates the advantage of cross-fitting in reducing overfitting bias

## Applications

- Causal inference from observational data  
- Econometrics and policy evaluation  
- Research settings requiring robust ATE estimation  

## File Overview

- `DML_RF.ipynb`: Contains the full pipeline for simulation, estimation, and comparison across the three ATE estimation methods.

## Requirements

- Python 3.8+
- `pandas`
- `numpy`
- `sklearn`
