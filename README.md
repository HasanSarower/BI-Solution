# BI Solution - Creating a simple datawarehouse pipeline for business.

Features:
Extraction:
Data extraction from csv is done by pyton panda module.Here data collected from csv areloaded into mysql database.
Before loading the csv data it checks whether similar data is already existed in database or not adn only extracts and load new data.

Transformation:
In this part data is cleaned and transformed into categories according to the need of our datawarehouse.All NANs are filled with zero and resampled the historical data into day/month/year.

Loading:
Transformed data is loaded into our datawarehouse so that necessary works for Business Intelligence like prediction, daily charts of transactions etc. can be done.

After that some reports are generated from datas of warehouse by the system and depicts with pdf at regular basis.

Altogether, a function named "etl()" is written which does the upper described works and the etl is run regularly with a schedular module.
Scheduler module link: https://github.com/dbader/schedule

Finally, some exploratory analysis is done to find trend,seasonal trend and anomaly and for prediction of volume of BTC for given timeframe OLS regression is carried out.

Technology stack:
Python modules:
pandas ,numpy,seaborn,matplotlib,sqlalchemy,statsmodels.formula.api
Database :
Mysql,mysqlWorkbench


 
 
