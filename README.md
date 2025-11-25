# Task-3-Finding-expiry-of-stock-
This project provides a simple Flask API to calculate weekly expiry dates for major Indian indices such as NIFTY, BANKNIFTY, and FINNIFTY.
The expiry day is decided based on the weekly expiry rule:

Index	Weekly Expiry
NIFTY	Thursday
BANKNIFTY	Wednesday
FINNIFTY	Tuesday

This API accepts the index name and a reference date and returns the next expiry date.

# Features

Simple and lightweight Flask API
Supports NIFTY, BANKNIFTY, FINNIFTY
Automatically calculates the nearest weekly expiry from the given date
Returns clean JSON response
Easy to test via browser or Postman

# How It Works

The API maps each index to its weekly expiry weekday
Converts the input date into a Python datetime
Calculates the number of days remaining until the expiry weekday
Returns the upcoming expiry date in YYYY-MM-DD format

Running the API

Install dependencies:
pip install flask
Run the app:
python app.py
Open in browser or Postman:
http://127.0.0.1:5000/expiry?index=NIFTY&date=2025-01-03
