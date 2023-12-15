The system is developed to automatically make stock holding recommendation each day before the trading hours. 
The recommendation is shown daily prior to the trading hours in a webpage that the user can access. 
The performance of the past recommendation is also shown against S&P 500 performance.


File:
final_eecs6893_port_opt_airflow_v2.py is used to run on the airflow including the following steps: /n
1  download the data from sources   /n
2  fit the machine learning model (XGBoost) and make the 1 day ahead prediction   /n
3  pull the news feed from finnhub and feed it into finBert   /n
4  run the weight recommendation based on Black-Litterman model   /n
5  send the report files to Google Cloud databucket for report shown in the website   /n
6  The report is shown on the website   /n
