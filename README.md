# 🚀 Task API

A RESTful Task Management API built using **FastAPI**, **PostgreSQL**, **SQLAlchemy**, and **Docker**.

## 📌 Features

- Create a Task
- Get All Tasks
- Get Task by ID
- Update Task
- Delete Task
- PostgreSQL Database
- Dockerized Application
- Layered Architecture (Repository + Service)

---

## 🛠️ Tech Stack

- Python 3.12
- FastAPI
- SQLAlchemy
- PostgreSQL
- Docker
- Docker Compose

---

## 📂 Project Structure

```
TaskAPI/
├── app/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── repository.py
│   ├── postgres_repository.py
│   └── service.py
│
├── sql/
│   └── init.sql
│
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/Punitgpatil925/task-api.git
cd task-api
```

---

### Create Environment File

Create a `.env` file in the project root.

```
DATABASE_URL=postgresql://postgres:password@db:5432/taskdb
```

---

### Run with Docker

```bash
docker compose up --build
```

---

## 📖 API Documentation

Swagger UI

```
http://localhost:8000/docs
```

---

## 📌 Available Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/tasks` | Get all tasks |
| GET | `/tasks/{task_id}` | Get task by ID |
| POST | `/tasks` | Create a task |
| PUT | `/tasks/{task_id}` | Update a task |
| DELETE | `/tasks/{task_id}` | Delete a task |

---

## 🧪 Example Request

### Create Task

```json
{
  "title": "Learn Docker"
}
```

### Response

```json
{
  "id": 1,
  "title": "Learn Docker",
  "done": false
}
```

---

## 🐳 Docker

Build and start the application:

```bash
docker compose up --build
```

Stop containers:

```bash
docker compose down
```

---

## 👨‍💻 Author

**Punit Patil**

