# Fuel Blend Prediction - RON Estimation

## Overview
This project predicts the **Research Octane Number (RON)** of fuel blends based on their composition. It uses advanced **machine learning models** and **non-linear feature engineering** to achieve high prediction accuracy. The pipeline is designed to handle volume- and mole-based features and incorporates feature optimization techniques inspired by industry best practices.

## Features
- Supports **volume- and mole-based fuel compositions** as input features.
- Predicts the **RON value** of the fuel blend.
- Implements multiple machine learning algorithms:
  - Linear models (OLS, Ridge, Lasso)
  - K-Nearest Neighbors (KNN)
  - Support Vector Machines (SVM)
  - Decision Trees
  - Random Forests
  - LightGBM (optimized with Optuna)
  - MLP with non-linear feature engineering
- Manual feature transformations and grouping (e.g., `BlendProperty7 ≈ 0.998 * BlendProperty3 + 0.0007`) to reduce prediction error.
- Hyperparameter tuning using **Optuna** for optimal model performance.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ESAIPREETHAM/Fuel-blend-Prediction-model.git
   cd fuel-blend-prediction
