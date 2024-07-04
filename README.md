# Automatic Weather Station

This project is an Automatic Weather Station designed to monitor, collect, and analyze weather data such as temperature, pressure, wind strength, direction, and precipitation. The collected data is stored in a MySQL database and made available through a graphical interface and a web application. The project leverages a combination of a weather data simulator and the OpenWeather API for real-time updates.

## Project Overview

The Automatic Weather Station system involves the following components:

- **Backend:** Python with Flask for the web application and MySQL for data storage.
- **Frontend:** HTML, CSS, and JavaScript for the user interface.
- **Weather Data:** Simulated data and real-time data from the OpenWeather API.

## Features

- Real-time weather data fetching from the OpenWeather API.
- Storage of weather data in a MySQL database.
- Web interface to display weather data and fetch updates for different cities.

## Prerequisites

Ensure that the following are installed on your system:

- Python 3.x
- MySQL
- Git (optional, for cloning the repository)

## Step-by-Step Process to Execute the Project

### 1. Download and Extract the Project

Download the `weather-monitoring-system.zip` file and extract its contents to a directory on your local machine.

### 2. Set Up the Virtual Environment

Open a terminal or command prompt and navigate to the project directory:

```sh
python -m venv venv
Activate the virtual environment:

sh
Copy code
venv\Scripts\activate   # On Windows

3. Install the Dependencies
Install the required Python packages using requirements.txt:

sh
Copy code
pip install -r requirements.txt

4. Set Up the MySQL Database
Open your MySQL client (e.g., MySQL Workbench or MySQL command line).

Execute the create_database.sql script to create the database and table:

Using MySQL command line:
sh
Copy code
mysql -u root -p < create_database.sql

Using MySQL Workbench:
Open a new SQL tab.
Copy and paste the contents of create_database.sql.
Execute the script.

5. Fetching Weather Data
Open a new terminal or command prompt.

Navigate to the project directory and activate the virtual environment (if not already activated):

sh
Copy code
venv\Scripts\activate   # On Windows
Run the weather data fetch script:

sh
Copy code
python fetch_weather.py

6. Running the Flask Application
Ensure the virtual environment is activated.

Run the Flask application:

sh
Copy code
python app.py
Open a web browser and navigate to: http://127.0.0.1:5000

You should see the weather monitoring application. You can input a city name to get real-time weather updates.

Usage
Homepage: The homepage displays the weather data for a default city.
City Input: Enter the name of any city in the input box and click "Get Weather" to fetch the real-time weather data for that city.
Project Structure
app.py: The main Flask application.
fetch_weather.py: Script to fetch and store weather data.
create_database.sql: SQL script to set up the MySQL database and tables.
templates/: Directory containing HTML templates.
static/: Directory containing static files (CSS, JS).
requirements.txt: List of Python dependencies.
License
This project is licensed under the MIT License. See the LICENSE file for details.