**Lufthansa Stock Price Prediction

This project is a machine learning model designed to predict Lufthansa's future stock prices using two approaches:
1. **Linear Regression** to predict the actual future stock prices (numerical values).
2. **Random Forest** classifier to predict whether the stock price will go **UP** or **DOWN**.

## Features

- **Linear Regression**: Predicts the actual stock price for the next 7 days.
- **Random Forest**: Predicts the stock price movement (UP or DOWN) for the next 7 days.
- Uses historical stock data such as **Open**, **High**, **Low**, **Volume**, **Moving Averages (MA5, MA20)**, and **RSI** (Relative Strength Index).
- The data includes feature engineering, model training, and predictions for both approaches.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Load the notebook `lufthansa.ipynb` in a Jupyter environment.
2. The notebook automatically reads and preprocesses historical stock data.
3. The stock price for the next 7 days is predicted using **Linear Regression** (numerical value) and **Random Forest** (UP/DOWN movement).

To run the notebook:

```bash
jupyter notebook lufthansa.ipynb
```

## Model Overview

### Data Preprocessing
- The historical stock data is processed and new features are created, such as:
  - **Moving Averages**: MA5 (5-day moving average), MA20 (20-day moving average)
  - **RSI**: Relative Strength Index, a momentum indicator
- The features are then used to train two models: **Linear Regression** for numerical predictions and **Random Forest** for classification.

### Linear Regression Model
- **Objective**: Predict the actual stock prices for the next 7 days.
- **Model**: A simple linear regression model is trained on historical stock data to forecast future prices.
- **Prediction Output**: The model provides numerical predictions for each of the next 7 days.

### Random Forest Classifier Model
- **Objective**: Predict whether the stock price will increase or decrease in the next 7 days.
- **Model**: A Random Forest classifier is used to classify the future stock price movement (UP or DOWN) based on historical data.
- **Prediction Output**: The model outputs whether the stock price will rise ("UP") or fall ("DOWN") for the next 7 days.

## Example Output

### Linear Regression (Numerical Prediction)
```bash
Predicted stock prices for the next 7 days:
2024-09-21: 9.45
2024-09-22: 9.50
2024-09-23: 9.40
2024-09-24: 9.38
2024-09-25: 9.42
2024-09-26: 9.35
2024-09-27: 9.33
```

### Random Forest (UP/DOWN Prediction)
```bash
Predictions for stock price movement in the next 7 days:
2024-09-21: DOWN
2024-09-22: DOWN
2024-09-23: DOWN
2024-09-24: DOWN
2024-09-25: DOWN
2024-09-26: DOWN
2024-09-27: DOWN
```

## Dependencies

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib

## License

This project is licensed under the MIT License.

