# Weather Data ETL Pipeline

## Project Overview

This project implements a simple Extract, Transform, Load (ETL) pipeline to fetch live weather data from the Open-Meteo API, process it, and store it locally in a CSV file. It's designed to be a foundational example for data extraction, cleaning, and persistence, demonstrating a basic data engineering workflow.

## Features

- **Extract**: Fetches current weather conditions (temperature, wind speed, weather code) for a specified city (currently hardcoded to Amsterdam) using the Open-Meteo API.
- **Transform**: Cleans and structures the raw JSON data into a flat Pandas DataFrame, performing data type conversions and basic quality checks (e.g., ensuring temperature is numeric).
- **Load**: Appends the processed weather data to a local CSV file (`daily_weather_log.csv`), creating the file if it doesn't exist.
- **Robust Error Handling**: Includes checks for API request failures and data anomalies during transformation.
- **Modular Design**: The pipeline is broken down into distinct `extract`, `transform`, and `load` functions for clarity and maintainability.

## Getting Started

### Prerequisites

To run this project, you'll need:

- Python 3.8+
- `requests` library
- `pandas` library

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Mozhan/ETL_pipeline_examples.git
    cd weather-data-etl
    ```

2.  **Install dependencies:**

    ```bash
    pip install requests pandas
    ```

### Usage

To run the ETL pipeline, simply execute the main Python script:

```bash
python your_etl_script_name.py # Replace 'your_etl_script_name.py' with your actual file name
