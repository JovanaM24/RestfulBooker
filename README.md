# Restful Booker API Collection

This repository contains the Postman collection and environment files for testing the **Restful Booker API**. The collection includes various API tests for the Restful Booker service. The tests are designed to validate the functionality of the API endpoints.

## Requirements

To run the tests, you need the following:

- **Newman**: A command-line tool for running Postman collections.
  - Install Newman globally using npm:
    ```bash
    npm install -g newman
    ```

- **Newman Reporters**: To generate CLI and HTML reports, install the required reporters.
  - Install the `newman-reporter-htmlextra` reporter globally:
    ```bash
    npm install -g newman-reporter-htmlextra
    ```

- **Postman Collection**: The `RestfulBooker.postman_collection.json` file, which includes a set of API tests.
- **Postman Environment**: The `RestfulBooker.postman_environment.json` file, which defines the environment settings for the API tests.

## Running the Tests

You can execute the tests using Newman with the following command:

```bash
newman run D:\RestfulBooker\RestfulBooker.postman_collection.json \
--environment D:\RestfulBooker\RestfulBooker.postman_environment.json \
--insecure \
--disable-unicode \
--reporters=cli,htmlextra \
--reporter-htmlextra-darkTheme
