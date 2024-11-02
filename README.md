# Data Driven Testing Framework (DDTF) with Selenium and Pytest

This project implements a Data Driven Testing Framework (DDTF) using Selenium WebDriver and Pytest to automate login tests for the Orange HRM portal. The test data is stored in an Excel file, and results are recorded back into the same file.


## Requirements

Ensure you have the following packages installed:

```bash
    pip install selenium openpyxl webdriver-manager pytest
```
## Excel File Structure
The Excel file Test_plan.xlsx contains the following columns:

**Test_ID: Unique identifier for each test case**
Username: Username for login
Password: Password for login
Date: Date of the test execution (automatically updated)
Time of Test: Time of test execution (automatically updated)
Name of Tester: Name of the tester (automatically set to "Aparna")
Test Result: Result of the test (Passed or Failed)

## Usage
Update Test Cases: You can add or modify test cases directly in the Test_plan.xlsx file.

Run the Tests: To execute the tests, run the following command in your terminal:

    ```bash
    pytest main.py

## Code Overview
* **excelfunctions.py**: Contains functions for reading test data from the Excel file and writing test results back to it.

* **locators.py**: Defines locators for the login page elements.

* **data.py**: Contains configuration data, including URLs and file paths.

* **main.py**: The main test logic that reads data from the Excel file, performs login actions, and writes results back.

## Test Cases
The tests will use the following credentials from the Excel file:

1. Admin / admin123
2. Aparna / admin123
3. Suman / admin123
4. admin123 / admin123
5. admin / Admin