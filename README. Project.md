# Amazon Stock Price Forecasting Using Statistical and Machine Learning Models

## Overview
This project predicts Amazon's stock prices using statistical models (ARIMA, SARIMA, Holt-Winters) and a machine learning model (FB Prophet). The dataset includes historical stock price data from May 1997 to October 2024, sourced from Yahoo Finance. The predictions focus on evaluating the performance and accuracy of these models.

## Features
- **Statistical Models**:
  - ARIMA (AutoRegressive Integrated Moving Average)
  - SARIMA (Seasonal ARIMA)
  - Holt-Winters Seasonal Model
- **Machine Learning Model**:
  - FB Prophet by Meta
- **Data Preprocessing**:
  - Handling missing values
  - Converting data types for time-series analysis
  - Visualizing trends and daily returns
- **Forecasting**:
  - Monthly aggregated stock prices
  - Forecasts for the period 2024-2028
- **Evaluation**:
  - Metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE)
  - Confidence intervals for predictions

## Dataset
- **Source**: [Yahoo Finance](https://finance.yahoo.com/)
- **Details**: Historical daily stock price data of Amazon from May 15, 1997, to October 2, 2024.
- **Fields**: Open, High, Low, Close, Adjusted Close, Volume.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/farhanmalik101/amazon_stock_price_project.git
   cd amazon_stock_price_project
   ```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
1. Open the amazon_stock_forecasting.ipynb file in Google Colab.
2. Upload the dataset (AMZN.csv) to the Colab environment.
3. Run the notebook cells sequentially for:
   - Data preprocessing
   - Exploratory data analysis
   - Forecasting using different models
   - Model evaluation and comparison
4. View plots and evaluation metrics for insights.

## Project Structure
- amazon_stock_forecasting.ipynb: Main Jupyter notebook for data preprocessing, modeling, and evaluation.
- requirements.txt: List of Python libraries needed for the project.
- AMZN.csv: Historical stock price dataset of Amazon (to be uploaded manually).
- README.md: This ReadMe file.


## Dependencies
The project requires the following Python libraries:

- pandas
- matplotlib
- scikit-learn
- pmdarima
- statsmodels
- prophet
Install all dependencies using:

```bash
pip install -r requirements.txt
```

## Results
- Best Model: FB Prophet outperformed ARIMA, SARIMA, and Holt-Winters in terms of MAE and MSE.
- Metrics Summary (2019–2024 evaluation period):
    - ARIMA: MAE = 34.37, MSE = 1719.18
    - SARIMA: MAE = 33.13, MSE = 1595.95
    - FB Prophet: MAE = 28.87, MSE = 1130.10
    - Holt-Winters: MAE = 33.14, MSE = 1592.69

## Contributing
Contributions are welcome. Feel free to open an issue or submit a pull request for improvements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
Special thanks to:

- Supervisor: Sunina Sharvy
- MSc Data Science Program, University of Hertfordshire
