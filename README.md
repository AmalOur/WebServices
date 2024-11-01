# WebServices Project

## Introduction
The WebServices Project is a RESTful API developed in Java using Spring Boot and Jersey. This application offers a complete set of CRUD functionalities for managing bank accounts (`Compte`).

## Features
- **API for Bank Accounts**: Supports create, read, update, and delete operations for bank accounts.
- **MediaType Compatibility**: Handles both JSON and XML data formats.
- **Spring Boot Framework**: Utilizes Spring Boot for streamlined setup and configuration.
- **Jersey REST Support**: Integrates Jersey for building RESTful endpoints.
- **H2 In-Memory Database**: Uses H2 for quick development and testing.
- **Lombok Library**: Reduces boilerplate code with easy-to-use annotations.

## Getting Started

### Requirements
- **Java** 17
- **Maven** 3.8.4 or above

### Installation

Clone the repository:

```bash
git clone https://github.com/amalour/webservices.git
cd webservices
```

Build the project:

```bash
mvn clean install
```

Run the application:

```bash
mvn spring-boot:run
```

## API Endpoints
- **Fetch Account by ID**: `GET /banque/compte/{id}`
- **Fetch All Accounts**: `GET /banque/comptes`
- **Create a New Account**: `POST /banque/compte`
- **Update an Account**: `PUT /banque/compte/{id}`
- **Delete an Account**: `DELETE /banque/comptes/{id}`

## Example API Requests

- **Fetch Account by ID**:

    ```bash
    curl -X GET "http://localhost:8082/banque/compte/1" -H "accept: application/json"
    ```

- **Create a New Account**:

    ```bash
    curl -X POST "http://localhost:8082/banque/compte" -H "accept: application/json" -H "Content-Type: application/json" -d "{ \"name\": \"John Doe\", \"balance\": 1000.0 }"
    ```

## Technologies Used
- Java 17
- Spring Boot
- Jersey
- Maven
- H2 Database (in-memory)
- Lombok

## Demo Videos
### JSON Format
https://github.com/user-attachments/assets/5242f34b-b3cf-4b09-960b-66b3368813c7

### XML Format
https://github.com/user-attachments/assets/3bc9d77a-6f19-4445-a4f8-2dad5286b0a8





---

