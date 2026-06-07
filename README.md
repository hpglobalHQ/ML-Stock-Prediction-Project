# ML-Stock-Prediction-Project

This project is a machine learning based stock prediction system that tries to predict stock movement using historical market data and technical indicators. Along with predictions, it also includes backtesting so the strategy performance can be checked on past data.

The main idea behind this project was to combine different ML models with feature engineering and create an interactive dashboard for analysis.

## Features

* Fetch stock data using Yahoo Finance
* Generate technical indicators automatically
* Train multiple models for prediction
* Ensemble approach using LSTM + XGBoost
* Backtesting with transaction costs and slippage
* Interactive dashboard using Streamlit
* Compare model performance with buy and hold strategy

---

## Project Structure

```bash

ML-Stock-Prediction-Project/
│
├── app.py                # Main Streamlit dashboard
├── backtest.py           # Backtesting functions and evaluation
├── data_pipeline.py      # Data collection and preprocessing
├── model.py              # Model training and prediction logic
├── requirements.txt      # Project dependencies
├── README.md
├── LICENSE
└── .gitignore
```

---

## Technologies Used

* Python
* Streamlit
* Pandas / NumPy
* Scikit-learn
* XGBoost
* PyTorch (for LSTM)
* Plotly
* Yahoo Finance API

---

## Installation

Clone the repository:

```bash
git clone <repo-url>
cd mlstockprediction
```

Create virtual environment:

```bash
python -m venv venv
```

Activate environment:

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Start the Streamlit app:

```bash
streamlit run app.py
```

After running the command, open the local URL shown in terminal.

---

## Workflow

### 1. Data Collection

Historical stock data is collected from Yahoo Finance.

### 2. Feature Engineering

Some indicators used:

* RSI
* MACD
* Moving averages
* Bollinger Bands
* Momentum indicators
* Volatility features

### 3. Model Training

The project uses multiple models:

* LSTM → captures sequential patterns
* XGBoost → handles non-linear relationships
* Ridge model → combines predictions

### 4. Backtesting

The strategy is evaluated using:

* Returns
* Sharpe ratio
* Drawdown
* Transaction cost impact
* Win rate

---

## Results

The goal is not only prediction accuracy but also checking whether predictions actually translate into profitable strategies after considering realistic market conditions.

---

## Limitations

* Market conditions change frequently
* Historical performance does not guarantee future returns
* Predictions should not be used directly for real trading decisions

---

## Future Improvements

Things that can still be improved:

* More advanced deep learning models
* Multi-stock portfolio support
* Live market integration
* Better explainability tools
* Model optimization

---

## Author

Made as a project to explore machine learning applications in stock market prediction and understand how different models perform in financial time series data.
