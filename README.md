# Population Manager API

Welcome to the Population Manager API! This API is designed to manage person and address information, allowing users to perform various operations related to population data using RESTful endpoints.

## Features

- **Create Person**: Add a new person to the database.
- **Create Multiple Persons**: Add a list of persons at once.
- **Create Address**: Add a list of addresses to the database.
- **Retrieve Person by ID**: Get details of a person using their unique ID.
- **Retrieve All Persons**: Get a list of all persons in the database.
- **Update Person**: Modify the details of an existing person.
- **Update Address**: Modify the details of an existing address.
- **Delete Person**: Remove a person from the database using their ID.
- **Delete Address**: Remove an address from the database using its ID.
- **Clear All Persons**: Remove all persons from the database.

## Requirements

- **Java Version**: This project requires Java 11 or later.
- **Spring Boot**: The application is built using Spring Boot. Ensure you have the necessary dependencies configured in your `pom.xml` or `build.gradle`.

## Installation

To get started with the Population Manager API, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/alesiopuf/population-manager-api.git

2. **Navigate the project directory**:
   ```bash
   cd population-manager-api

3. **Build the application**:
   If you have Maven run:
   ```bash
   mvn clean install

 4. **Run the application**:
    To start the API server, use the following command:
    ```bash
    mvn spring-boot:run
    ```
    Or if you have a runnable jar:
    ```bash
    java -jar target/population-manager-api.jar

## Usage

Once the API is running, you can access the following endpoints:
- POST /person: Create a new person (requires JSON body).
- POST /persons: Create multiple persons (requires JSON body).
- POST /address: Create multiple addresses (requires JSON body).
- GET /persons/{id}: Retrieve a specific person by ID.
- GET /persons: Retrieve all persons.
- PUT /persons/{id}: Update an existing person (requires JSON body).
- PUT /address/{id}: Update an existing address (requires JSON body).
- DELETE /persons/{id}: Delete a person by ID.
- DELETE /address/{id}: Delete an address by ID.
- DELETE /persons: Clear all persons from the database.

## Example Requests

1. **Create new person**:
   ```bash
   curl -X POST http://localhost:8080/person -H "Content-Type: application/json" -d '{"firstName": "John", "lastName": "Doe"}'

2. **Retrieve all persons**:
   ```bash
   curl -X GET http://localhost:8080/persons

3. **Update a person**:
   ```bash
   curl -X PUT http://localhost:8080/persons/1 -H "Content-Type: application/json" -d '{"firstName": "Jane", "lastName": "Doe"}'

4. **Delete a person**:
   ```bash
   curl -X DELETE http://localhost:8080/persons/1

## Contribution Guidelines

Contributions are welcome from anyone interested in improving the application.
Contribution avenues include:
- Writing tests to ensure application stability and reliability.
- Enhancing specifications for better understanding and maintainability.
- Identifying and resolving bugs to improve the overall quality.
- All pull requests must undergo review by the repository owner before merging.

## Contact Information

- For inquiries or support related to the Population Manager App, please contact:
- Email: alesiopuf@yahoo.com
- Email title: 'Population Manager API Support'

---

Ensure to follow the setup instructions carefully to deploy the application successfully.
