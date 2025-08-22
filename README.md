# 160923733118-Syed-Abdur-Rasheed

Project Description

This project is a Spring Boot REST API designed to manage tasks.
It provides basic CRUD functionality (Create, Read, Update, Delete) using an in-memory data store rather than a database.

Project Structure
Task (Model)

A Java class representing a task.

Fields include: id, title, description, and status.

Includes standard getters, setters, and toString() methods.

Status (Enum)

Defines valid states for a task.

Possible values: TODO, IN_PROGRESS, COMPLETED, BLOCKED.

TaskService (Service Layer)

Acts as the business logic of the application.

Uses a Map<Long, Task> to store tasks, simulating persistence.

Provides operations for creating, retrieving, updating, and deleting tasks.

TaskController (REST Controller)

Exposes REST endpoints under the base path /tasks.

Annotated with @RestController and @RequestMapping.

Endpoints available:

POST /tasks → Create a new task

GET /tasks/{id} → Fetch a task by ID

GET /tasks → Fetch all tasks

PUT /tasks/{id} → Update an existing task

DELETE /tasks/{id} → Remove a task

API Testing with Postman

You can test all endpoints easily using Postman:

Open Postman → Go to Collections → Click + (New Collection).

Add a request and configure it as per the endpoint you want to test.