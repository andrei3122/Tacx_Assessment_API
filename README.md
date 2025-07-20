# Tacx API Assessment – Postman Test Suite

This repository contains a set of automated test cases written in Postman for the dummy REST API at "https://dummy.restapiexample.com"

## Test Suite Overview

The collection includes tests for the following HTTP methods:
- **GET**: Fetch all employees and a single employee by ID
- **POST**: Create a new employee
- **PUT**: Update an employee's information
- **DELETE**: Delete an employee by ID

Each request contains tests written in the **Tests** tab of Postman using JavaScript. Tests validate:
- Response codes (e.g., 200, 401, 429)
- Response time (<2000ms)
- JSON format
- Field-level validations (e.g., "employee_name", "employee_salary", etc.)

## Files Included
- "Tacx_Assessment.postman_collection.json": The Postman test collection

## How to Run the Scripts
1. **Install [Postman]**(https://www.postman.com/downloads/)
2. **Import the collection**:
   - Open Postman
   - Click "Import"
   - Click "Upload Files"
   - Select the "Tacx_Assessment.postman_collection.json" file
4. **Run each request manually**
   - Or use the Collection Runner to run all at once

## Notes
- Please note that due to many people accessing this website for testing purpouses, the code may fail due to error 429 "Too Many Requests". If this happens, wait 30 seconds and retry running the code.
- This API is a dummy site, so some endpoints (e.g., DELETE) return success even for non-existent IDs.
