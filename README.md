# Delivery Time Regression

Neural-network based delivery time prediction project built using TensorFlow/Keras, and hyperparameter tuning with keras_tuner and finally SHAP analysis as well.

- You can find the entire workflow in: `nn_delivery_time_regression.ipynb`.
- Best model will be saved as: `best_nn_model.keras`
- Keras Tuner outputs are saved to: `kt_tuning/` (however, not included in this repo)
- Artifacts will be saved to: `artifacts/` (however, they are not included in this repo)

Clone the repo, run the notebook locally top to bottom and you will have all the files saved.

## Overview

This project predicts delivery_time_mins from order, market, and dasher related features.

The workflow includes:
- data loading and validation
- leakage-safe feature engineering and preprocessing
- neural network training and evaluation
- linear baseline comparison
- permutation importance and SHAP explainability
- artifact export for reuse in inference

## Main Assets

- Notebook: `nn_delivery_time_regression.ipynb`
- Once you run the notebook, you will have the following artifacts ready for deployment:
  - artifacts/delivery_time_nn.keras
  - artifacts/feature_engineer.joblib
  - artifacts/preprocessor.joblib
  - artifacts/metadata.json

## Current Model Performance

From the latest notebook run:
- Final NeuralNet test MAE: ~3.87 minutes
- Final NeuralNet test RMSE: ~4.94 minutes
- Final NeuralNet test R2: ~0.72


