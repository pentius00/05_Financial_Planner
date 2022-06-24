# Financial_Planner
**Visualize savings and forecast future performance using Alpaca API and Monte Carlo simulation.**

---
## Technologies
Code is written using Python version 3.7 and runs in a Jupyter Lab notebook. 
The following libraries are required to run this program:

- [Datetime](https://docs.python.org/3/library/datetime.html) supplies classes for manipulating dates and times.
```python
import datetime as dt
```
- The [OS](https://docs.python.org/3/library/os.html) module is used to interact with the computer's operating system.
```python
import os
```
- [Pandas](https://pandas.pydata.org/docs/) is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.
```python
import pandas as pd
```
- [Requests](https://docs.python-requests.org/en/master/) Requests is an elegant and simple HTTP library for Python, built for human beings.
```python
import requests
```
- [JSON](https://docs.python.org/3/library/json.html) is a lightweight data interchange format inspired by JavaScript object literal syntax.
```python
import json
```
- [Python-dotenv](https://github.com/theskumar/python-dotenv) gets and sets values in a .env file in local and production servers.
```python
from dotenv import load_dotenv
```
- [Alpaca](https://alpaca.markets/docs/) API is a modern platform for algorithmic trading.
```python
import alpaca_trade_api as tradeapi
```
- MCForecastTools is a Python class for runnning Monte Carlo simulation on portfolio price data. View the file and read the docstring [here](https://github.com/rdillens/05_Financial_Planner/blob/main/MCForecastTools.py).
```python
from MCForecastTools import MCSimulation
```

---
## Inatallation Guide
- Alpaca
The Alpaca API requires an access token, which can be obtained by creating an account [here](https://alpaca.markets/).
```powershell
pip install alpaca-trade-api
```
- Python-dotenv
Use python-dotenv to save the API access token as a key-value pair in a hidden file named `.env`. Be sure to enclose the access token value in double quotation marks `""` and do not use any spaces.
```powershell
pip install python-dotenv
```

---
## Usage
### Part 1: Create a Financial Planner for Emergencies
The first part of this program defines the number of bitcoin and etherium tokens in a user's wallet and the users's monthly income.
```python
btc_coins = 1.2
eth_coins = 5.3
monthly_income = 12000
```
Using the Free Crypto API, the JSON response for each requested currency is stored and displayed and the current value of the user's wallet is calculated.
Then, the program defines the number of shares held in stocks and bonds in the SPDR S&P 500 ETF Trust (ticker: SPY) and of the iShares Core US Aggregate Bond ETF (ticker: AGG). Using the Alpaca API, the closing value of the previous trading day is used to calculate the current value of the user's savings portfolio.
Lastly, a pie chart is produced showing the ratio of crypto to stocks and bonds and the total value of the portfolio is compared to three months of income to determine if the user's portfolio is large enough to fund the emergency portfolio. 
### Part 2: Create a Financial Planner for Retirement
Part two begins by gathering 10 years of historical closing prices using the Alpaca API. 
Then, a Monte Carlo simulation is used to predict the value of the portfolio after 30 years with a 60/40 split between stocks/bonds and after 10 years of an 80/20 split. Results are plotted and future value is calculated within a 95% confidence interval. 
Finally, an evaluation is made to determine if the user could potentially retire after 10 years. 

---
## Examples
![JSON response](/Images/JSON_response_BTC.png)
![Alpaca Dataframe](/Images/Alpaca_df.png)
![10 Year Historical Dataframe](/Images/Historical_df.png)
![Portfolio Pie Chart](/Images/Port_Pie.png)
![Monte Carlo Line Plot](/Images/MCS_30_Years.png)
![Monte Carlo Histogram](/Images/Dist_Hist.png)

---
## Contributors
Starter code was given in the Rice FinTech Bootcamp and all modifications were made by Remy Dillenseger.

---
## License
This project is licensed under the MIT License.
[Click Here](https://github.com/rdillens/05_Financial_Planner/blob/main/LICENSE) for more information.
