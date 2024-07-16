
---

# Gold Price Prediction Using Machine Learning

## Abstract

Historically, gold has been a significant form of investment globally, retained by central banks to guarantee external debt servicing and manage inflation. This project focuses on predicting future gold prices using Machine Learning techniques, specifically Linear Regression (LR). Data from the largest gold ETF (GLD) spanning from November 2004 to January 2024 is utilized for analysis and model development.

## Methodology

### Step-by-Step Approach:

1. **Data Collection and Preprocessing:**
   - Data is sourced from [ETF.com/GLD](http:/www.etf.com/GLD) covering the period from November 2004 to January 2024.
   - Preprocessing involves cleaning data by removing irrelevant columns and handling missing values using `dropna()`.

2. **Feature Engineering:**
   - Explanatory variables (features) include moving averages (e.g., 5-day, 10-day) of the Gold ETF prices.
   - Additional variables like prices of related ETFs (e.g., GDX, USO) or economic indicators can be incorporated for enhanced prediction.

3. **Model Development:**
   - Splitting data into training and test sets (75% training, 25% testing).
   - Implementing Linear Regression model using `scikit-learn`.
   - Training the model on the training dataset to establish coefficients and constants.

4. **Prediction:**
   - Using the trained model to predict future Gold ETF prices based on the explanatory variables.
   - Evaluating model performance using metrics such as accuracy, precision, recall, and F1-score.

5. **Cumulative Returns Analysis:**
   - Calculating daily percentage changes in Gold ETF prices.
   - Creating trading signals based on predicted price movements.
   - Computing cumulative returns to assess the effectiveness of the prediction strategy.

## Implementation Details

- **Libraries Used:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`.
- **Python Version:** Python 3.x.
- **Dataset:** ETF data collected from [ETF.com/GLD](http:/www.etf.com/GLD).

## Result

The regression model outputs the predicted Gold ETF price based on the following equation:
**Gold ETF Price (y)=1.17×5 Days Moving Average (x1)−0.17×10 Days Moving Average (x2)+0.22**

![ The graph above shows the expected and actual Gold ETF price.](main/Picture1.png)


## Conclusion

This project aims to demonstrate the application of Machine Learning, specifically Linear Regression, in predicting Gold ETF prices. By leveraging historical data and appropriate features, the model seeks to provide insights into future price trends, aiding investors in making informed decisions.




---

