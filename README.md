# climate_sql_database_project

This project uses SQLAlchemy ORM queries in Python to explore and analyze climate data of a SQL database containing temperature and precipitation data of Honolulu. Visualizations are created mostly using pandas and matplotlib. SQLAlchemy is a SQL toolkit in Python that allows control of SQL database in Python scripts.

This project also designs a Climate web application using Flask API, a micro web framework written in Python. The Flask application talks to the climate database through SQLAlchemy, queries the data, and displays the results in json format.

## Required Python packages

- matplotlib
- pandas
- numpy
- datetime
- sqlalchemy
- flask

## Navigation
- climate.ipynb contains analysis of climate data from the SQL database
- hawaii.sqlite is the database. You can use [DB Browser for SQLite](https://sqlitebrowser.org/) to view the the database.
- hawaii_api.py is Climate web APP created using Flask

## Database Description

The database contains two data tables, measurement and station.
- measurement
  - prcp column is precipitation data
  - tobs column is temperature observation data

## Instructions for Running and navigating Flask API

Store the repository in a local folder. Double-click on hawaii_api.py and, if run correctly, the last line should read: `Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)`. Open your browser and type `http://127.0.0.1:5000/`. You should be able to see the following: 
  ```
Available Routes:
Precipitation data recorded in last two years: /api/v1.0/precipitation
List of all recorded stations: /api/v1.0/stations
Temperature data recorded in last two years: /api/v1.0/tobs
Replace 'start_date' with a date in the format 'yyyy-mm-dd' for temperature data after that date: /api/v1.0/start_date
Replace 'start_date' and 'end_date' with specific dates for temperature data in that date range: /api/v1.0/start_date/end_date
```
Then, to assess precipation route, add `/api/v1.0/precipitation` at the end of `http://127.0.0.1:5000/`.

