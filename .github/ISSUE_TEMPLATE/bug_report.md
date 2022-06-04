---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

**Describe the bug**
A clear and concise description of what the bug is.
When using the Client API and requesting historical_klines with a limit of 10 the function loops forever.

**To Reproduce**
Code snippet to reproduce the behavior:

from binance.client import Client

timestamp = client._get_earliest_valid_timestamp(symbol=SYMBOL, interval='1d')
msg = client.get_historical_klines('BTCUSDT', '1d', timestamp, limit=10)

**Expected behavior**
A clear and concise description of what you expected to happen.
It should return a list of 10 OHLCV values or throw an exception stating it's invalid request (i.e wrong parameters, invalid timestamp, type error, etc).

**Environment (please complete the following information):**
 - Python version: [e.g. 3.5]
 - Python version 3.8
 - Virtual Env: [e.g. virtualenv, conda]
 - Virtualenv
 - OS: [e.g. Mac, Ubuntu]
 - Windows
 - python-binance version
 - 0.3

**Logs or Additional context**
Add any other context about the problem here.
There is no log at all since the function is executing forever. 
I also have a solution for you. please send me an email and ill send the solution if needed.
