# sqlalchemy-challenge
Repo for Challenge 10

# Weather Data Analysis and API

## Overview
This project includes a Jupyter notebook and a Flask API designed to analyze weather data and provide access to the data through a set of API endpoints. 

## Notebook
The Jupyter notebook (`climate_starter.ipynb`) contains an exploratory analysis of weather data, focusing on precipitation and station activity. It uses SQLAlchemy ORM to interact with a SQLite database and Pandas for data manipulation and visualization with Matplotlib.

### Features
- Reflects tables into SQLAlchemy ORM.
- Queries the most recent date and retrieves the last 12 months of precipitation data.
- Plots precipitation data over time.
- Calculates summary statistics for precipitation.
- Identifies the most active weather stations and their temperature observations.
- Plots temperature observations as a histogram.

## Flask API
The Flask application (`app.py`) provides a web server with a set of API endpoints that return JSON representations of the weather data.

### Endpoints
- `/`: Home page listing all available routes.
- `/api/v1.0/precipitation`: Returns JSON representation of precipitation data.
- `/api/v1.0/stations`: Returns a list of weather stations.
- `/api/v1.0/tobs`: Returns temperature observations for the most active station.
- `/api/v1.0/temp/start`: Returns min, avg, and max temperatures for all dates greater than or equal to the start date.
- `/api/v1.0/temp/start/end`: Returns min, avg, and max temperatures for dates between the start and end date.

## Installation
To run the notebook and API, you will need to install the required Python packages:

#```bash
pip install numpy pandas matplotlib sqlalchemy flask

## Usage
To launch the notebook, run: jupyter noebook climate_starter.ipynb

To start Flask API, run: FLASK APP=App.py flask run

## Data
The data for this project is stored in the Resources folder, containing hawaii.sqlite, hawaii_measurements.csv, hawaii_stations.csv.
