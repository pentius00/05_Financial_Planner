# 05_Financial_Planner
**Visualize savings and forecast future performance using Alpaca API and Monte Carlo simulation.**

## Technologies
Code is written using Python version 3.7 and runs in a Jupyter Lab notebook. 
The following libraries are required to run this program:

- [Datetime](https://docs.python.org/3/library/datetime.html) provides functions for working with dates and times such as getting the current date and last trading day.
```python
import datetime as dt
```
- The [OS](https://docs.python.org/3/library/os.html) module is used to interact with the computer's operating system.
```python
import os
```
- [Pandas](https://pandas.pydata.org/docs/) can be installed with Anadonda or PyPi.
```python
import pandas as pd
```
- Requests library helps access data via APIs.
```python
import requests
```
- JSON library parses API responses into a human-readable format.
```python
import json
```
- Python-dotenv library is used to read key-value pairs from hidden files.
```python
from dotenv import load_dotenv
```
- Alpaca API SDK for stock trading information. Its use requires an API key, obtained from the Alpaca website.
```python
import alpaca_trade_api as tradeapi
```
- A Python class for runnning Monte Carlo simulation on portfolio price data. 
```python
from MCForecastTools import MCSimulation
```

---

## Inatallation Guide

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
[Click Here](https://github.com/rdillens/05_Financia_Planner/blob/main/LICENSE) for more information.