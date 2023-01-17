# StableUnstable_ElectricityPriceForecasting

One of our roles in the EU IMPROVEMENT [EU IMPROVEMENT](https://projects2014-2020.interregeurope.eu/improve/ "EU IMPROVEMENT") project is to develop accurate
data-driven techniques for predicting the hourly market price
of electricity in Portugal. By examining the literature, we have
identified a large panoply of studies dealing with the forecast
of energy prices. By deeply analyzing them, we realized that
they fail to address unstable market conditions. It appears that
each uses its own datasets and preparation processes to perform
a prediction. To overcome those two major limitations, we propose ten (10) AI techniques for the forecast of electricity prices using the same dataset related to the Portuguese market between 2017 and 2022. Our techniques are belonging to statistical, Machine Learning (ML), and Deep Learning (DL) approaches, at several temporal granularities (hourly, daily,
weekly, and monthly). The 10 techniques are implemented, tested, and evaluated with the MAE, RMSE, and CV metrics.

## Software requirements
All algorithms have been implemented using Google Collab notebooks currently running : 

| Tool | version    | 
| :---:   | :---: | 
| Python  |  3.7.13  | 
| tensorflow |  2.8.2  | 
| keras |  2.8.0  | 
| statsmodels | 0.13.2   |
| pandas |  1.3.5  | 
| matplotlib |  3.2.2  | 
|  sklearn |  1.0.2  | 
| numpy |  1.21.6  | 
| seaborn | 0.11.2   |
| scipy | 1.7.3  |   

## Reproduce our work

### Code
This repository contains the code of the algorithms used to implement electricity price forecasting as described in in the Paper - AI Approaches for Electricity Price Forecasting in
Stable/Unstable Markets: EU Improvement Project. 
We implemented and evaluate three classes
of AI techniques: statistical (STAT), Machine Learning (ML),
and Deep Learning (DL), and in each class we consider the
following methods: (i) STAT: ARIMA, HoltWinter, (ii) ML: Multiple Linear regression, SVM, Extreme Gradient Boosting, Random Forest and (iii) DL:
LSTM. All algorithms can be found in the src file.

### Dataset

The electricity prices of the Portuguese market are loaded
from the [Redes Energ ́eticas Nacionais (REN)](https://mercado.ren.pt/EN/Electr/MarketInfo/MarketResults/OMIE/Pages/Prices.aspx "REN") website.

The hourly generation by source data are gathered from the [ENTSO-E Transparency platform](https://transparency.entsoe.eu/ "ENTSO-E").

The data preprocessing we applied can be found [here](./src/data_study/.README.md).

### Results 

Here are all our results obtained with the differents algorithms using the entire dataset or only the 2017/2021 part. 
![alt text](/docs/img/statistical_results_tables.png)
![alt text](/docs/img/machine_learning_algorithms.png)
![alt text](/docs/img/deep_learnig_results.png)
