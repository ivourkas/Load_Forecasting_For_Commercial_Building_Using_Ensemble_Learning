# Load_Forecasting_For_Commercial_Building_Using_Ensemble_Learning

![Power Systems](https://img.shields.io/badge/Power-Systems-blue) ![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange) ![Energy Forecasting](https://img.shields.io/badge/Energy-Forecasting-green)

## Project Overview
This repository contains an ensemble-based short-term load forecasting (STLF) model for predicting hourly power consumption of Shepard Hall, a university building. The system combines Random Forest regression and LSTM networks with innovative ensemble strategies to achieve superior forecasting accuracy.

## Key Features
- **Hybrid Approach**: Combines white-box domain knowledge with data-driven ML
- **Ensemble Strategies**:
  - MSE-weighted average of predictions
  - Stacking-based meta-model (linear regression combiner)
- **Temporal Analysis**: Handles hourly consumption patterns and seasonal variations
- **Evaluation**: Real-world data from Feb 2020-Jan 2025 with Feb 2025 test set

## Abstract
Electricity load forecasting is critical for efficient power system operation, enabling optimal energy dispatch, cost reduction, and grid stability. Traditional white-box models require extensive domain expertise, whereas data-driven black-box approaches, such as machine learning, offer faster development cycles and adaptability. This paper presents an ensemble-based short-term load forecasting (STLF) model for predicting the hourly power consumption of Shepard Hall, a university building. We employ Random Forest (RF) regression and Long Short-Term Memory (LSTM) networks, leveraging their complementary strengths in handling nonlinear temporal dependencies. To further enhance accuracy, we introduce two ensemble strategies: (1) a mean squared error (MSE)-weighted average and (2) a stacking-based meta-model that combines RF and LSTM predictions via linear regression. Our experiments use real-world metered consumption data (Feb. 2020–Jan. 2025) for training and February 2025 for evaluation. Results demonstrate that the stacking ensemble outperforms individual models, achieving the lowest MSE. This work highlights the potential of hybrid machine learning approaches in building energy management systems.

**Index Terms**—Load forecasting, Random Forest, LSTM, ensemble learning, stacking, energy management.

## Repository Structure

├── data/ # Weather and consumption datasets
│ ├── Weather data 2020-02-01 to 2022-10-01.csv
│ ├── Weather data 2022-10-02 to 2025-01-31.csv
│ └── Weather_Test_Correct.csv
├── figures/ # Visualizations and analysis
│ ├── CCNY CLOSED DAYS.xlsx
│ ├── Evaluation Data Students_Shepard 2025.xlsx
│ ├── Model Development Data_Shepard 2025.xlsx
│ ├── Natural Gas (Henry Hub).csv
│ ├── consumption_clean.png
│ ├── consumption_with_outliers.png
│ ├── cr_matrix.png
│ ├── distribution_histogram.png
│ ├── feature_importance_rf.png
│ ├── lstm_vs_actual.png
│ ├── peaks.png
│ ├── rf_vs_actual.png
│ ├── train_test_split.png
│ ├── ts_cv.png
│ └── weighted_vs_actual.png
├── output/ # Forecast results
│ └── February_2025_Forecast.xlsx
├── Project3.ipynb # Main Jupyter notebook
└── Project_3.pdf # Full project report
