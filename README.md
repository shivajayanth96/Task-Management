# Task Management API

A Java Spring Boot backend for task management following Domain-Driven Design (DDD) principles.

## Features

- Create, retrieve, update, delete tasks
- List tasks sorted by due date
- In-memory persistence
- Validation for required fields and future due dates
- Unit and integration tests

## Requirements

- Java 26
- Maven 4.1
- Git (optional, for cloning the repository)

## Install dependencies

This project uses Maven to download and manage dependencies automatically. You can use the included Maven wrapper so you do not need a local Maven installation.

```bash
./mvnw clean install
```

If you prefer a local Maven install, run:

```bash
mvn clean install
```

## Build and run locally

Start the application:

```bash
java -jar Task-Management.jar
```

Once started, the API will be available at `http://localhost:8080`.

## API Endpoints

- `POST /tasks`
- `GET /tasks/{id}`
- `PUT /tasks/{id}`
- `DELETE /tasks/{id}`
- `GET /tasks`

Optional query parameters for list:

- `status` = PENDING, IN_PROGRESS, DONE

## Tests

```bash
mvn test
```
