# Online Queue Management System

## Overview

The Online Queue Management System allows teachers to create and manage queues for their students. Teachers can generate a unique queue code, which students use to join the queue. The system provides functionality for teachers to manage the order of students in the queue efficiently.

## Features

- **Queue Management**: Teachers can create queues, generate codes, and manage the order of students.
- **Student Access**: Students can join queues using the provided code.
- **Real-Time Updates**: The queue order can be updated in real-time by the teacher.

## Technology Stack

### Backend

- **Spring Boot**: For building the web application.
- **Hibernate**: For mapping database entities and database operations.
- **Spring Security**: For securing the application using JWT-based authentication with custom filters.
- **Flyway**: For managing database migrations.
- **PostgreSQL**: As the database.

### Frontend

- **Svelte**: For building reactive user interfaces.
- **Svelte Routing**: For managing application routes.

### Containerization

- **Docker**: Each part of the application is containerized.
- **Docker Compose**: To build and run the entire application stack together.

## Getting Started

### Prerequisites

Ensure you have Docker and Docker Compose installed on your machine.

### Installation

1. **Download the `docker-compose.yml` File**:
   ```bash
   git clone https://github.com/learning-kyljmeeski/online-queue.git
   cd online-queue
   ```

2. **Build the Docker Images**:
   ```bash
   docker-compose build
   ```

3. **Run the Application**:
   ```bash
   docker-compose up
   ```

The application will be available at `http://localhost:8080` by default.

## Project Structure

```plaintext
.
├── backend
│   ├── src
│   ├── Dockerfile
│   └── ...
├── frontend
│   ├── src
│   ├── public
│   ├── Dockerfile
│   └── ...
├── docker-compose.yml
└── README.md
```

### Backend

- **Spring Web**: Provides the foundation for creating the web application.
- **Spring Security**: Implements JWT-based authentication for securing endpoints.
- **Hibernate**: Manages database operations through JPA.
- **Flyway**: Handles database migrations to ensure consistent schema management.

### Frontend

- **Svelte**: For creating dynamic and responsive user interfaces.
- **Routing**: Handled by Svelte's built-in routing capabilities for smooth navigation.

### Docker

- **Dockerfile**: Each component (backend, frontend) has its own Dockerfile.
- **Docker Compose**: Orchestrates the building and running of the entire application stack.

## Usage

### Teacher

1. **Create a Queue**: Log in and create a new queue.
2. **Share Queue Code**: Share the generated code with students.
3. **Manage Queue**: View and manage the students in the queue.

### Student

1. **Join Queue**: Enter the queue code provided by the teacher to join the queue.
2. **Wait in Queue**: Wait for your turn as the teacher manages the queue.

## Security

- **JWT Authentication**: Ensures secure access to the application.
- **Custom Filters**: Handle authentication and authorization tasks.

## Database Migrations

- **Flyway**: Manages database versioning and migrations to keep the schema up to date.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions or feedback, please reach out to [your email/contact information].

---

Enjoy using the Online Queue Management System!
