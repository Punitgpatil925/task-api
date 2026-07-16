# Task API

A simple CRUD API built using FastAPI.

## Features

- Create a Task
- Read All Tasks
- Read Task by ID
- Update a Task
- Delete a Task
- Interactive Swagger Documentation

## Technologies

- Python
- FastAPI
- Uvicorn

## Installation

```bash
pip install fastapi uvicorn
```

## Run

```bash
uvicorn main:app --reload
```

## Swagger UI

Open:

```
http://127.0.0.1:8000/docs
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Home |
| GET | /health | Health Check |
| GET | /tasks | Get All Tasks |
| GET | /tasks/{task_id} | Get Task by ID |
| POST | /tasks | Create Task |
| PUT | /tasks/{task_id} | Update Task |
| DELETE | /tasks/{task_id} | Delete Task |

## Author

Punit Patil