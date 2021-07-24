# 05_Financial_Planner
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
- Pandas
```powershell
pip install pandas
```
- Requests
```powershell
python -m pip install requests
```
- Python-dotenv
```powershell
pip install python-dotenv
```
- Alpaca
```powershell
pip install alpaca-trade-api
```

---
## Usage

---
## Examples

---
## Contributors
Starter code was given in the Rice FinTech Bootcamp and all modifications were made by Remy Dillenseger.

---
## License
This project is licensed under the MIT License.
[Click Here](https://github.com/rdillens/05_Financial_Planner/blob/main/LICENSE) for more information.