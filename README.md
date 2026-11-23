# Stock Price Prediction Using XGBoost

A machine learning project that predicts Tesla (TSLA) stock closing prices using an XGBoost Regressor and historical stock market data.

## Project Overview

This notebook explores Tesla stock data, visualizes price and trading-volume patterns, and trains a regression model to estimate the closing price (`Close`) using these input features:

- `Open`
- `High`
- `Low`
- `Volume`

The dataset is split into training and testing sets (80% / 20%). The model's predictions are evaluated using Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² score. The notebook also calculates an approximate accuracy-like percentage based on MAE; this is not a standard classification accuracy metric.

## Project Files

- `Stock_market_prediction_using_xgboost.ipynb` — Jupyter Notebook containing data exploration, visualizations, model training, prediction, and evaluation.
- `TSLA.csv` — Required input dataset (must be added to the repository or obtained separately).

## Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost

## Setup and Run

1. Clone or download this repository.
2. Install the required packages:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
   ```

3. Place `TSLA.csv` in the same directory as the notebook.
4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Stock_market_prediction_using_xgboost.ipynb` and run the cells in order.

## Dataset Requirements

The notebook reads a file named `TSLA.csv` and expects columns named `Date`, `Open`, `High`, `Low`, `Close`, and `Volume`. The CSV dataset was not included with the uploaded notebook, so it must be supplied before the notebook can run from the beginning.

## Notes

- This is an educational machine learning project, not financial advice or a tool for making investment decisions.
- Stock prices are uncertain; model predictions do not guarantee future performance.
- Before running the notebook, check the NumPy import in the first cell: it should be `import numpy as np` because later cells use `np.mean()`.
