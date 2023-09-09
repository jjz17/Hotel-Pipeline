# Hotel-Pipeline
A data pipeline for processing hotel booking demand data using Apache Airflow and Docker.

## Usage
### Initial Setup
1. (Generate env file) ```echo -e "AIRFLOW_UID=$(id -u)" > .env```
2. (Set up virtual environment)
   1. ```python3 -m venv .venv```
   2. ```. .venv/bin/activate```
   3. ```pip install -r ./requirements.txt```
3. (Set up databases and create user account) ```docker-compose up airflow-init```
   
### General Setup
1. (Start all services) ```docker-compose up```
   1. (Monitor container health in another terminal window) ```docker ps```
2. Visit [airflow UI](http://localhost:8080) with default credentials (username/password): airflow/airflow
3. (Shut down all services) ```docker-compose down```
