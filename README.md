# Weather ETL Pipeline
An Apache Airflow pipeline that pulls weather data from OpenWeatherMap API, processes it, and stores it in a Amazon S3 bucket.

## What It Does

This DAG runs daily to:
1. Check if the OpenWeatherMap API is available
2. Fetch current weather data for Portland
3. Convert temperatures from Kelvin to Fahrenheit
4. Save the processed data as a CSV file in an S3 bucket

## Prerequisites
- AWS acct
- OpenWeatherMap API key

Each file contains:
- City name
- Weather description
- Temperature (current, feels like..., min, max)
- Pressure and humidity
- Wind speed
- Timestamp and sunrise/sunset times
