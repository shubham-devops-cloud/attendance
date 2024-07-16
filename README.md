# Attendance

Attendance is a microservice which is designed in Python to manage employee's attendance information.

## Database

- Attendance application store information in MySQL database

## Environment Variable

| **ENVIRONMENT VARIABLE** | **DESCRIPTION**            |
|--------------------------|----------------------------|
| CONFIG_FILE              | Path of configuration file |

## Endpoints

The available endpoints for this application are:-

| **ENDPOINT**           | **REQUEST TYPE** | **DESCRIPTION**                                                                                               |
|------------------------|------------------|---------------------------------------------------------------------------------------------------------------|
| `/attendance/create`   | POST             | create endpoint collects the JSON payload of request and write the data to MySQL.                             |
| `/attendance/search`   | GET              | search endpoint fetch the information from MySQL server and return the JSON reponse.                          |
| `/attendance/healthz`  | GET              | healthz endpoint checks the DB connectivity and tells that application is ready to serve the requests or not. |