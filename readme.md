# 📝 FastAPI To-Do CRUD API

A beginner-friendly **FastAPI project** that demonstrates how to build a **RESTful API** with **CRUD operations**, **request/response validation using Pydantic**, and **in-memory data storage**. This project is ideal for learning **Web APIs**, **microservices basics**, and how ML models are later exposed via APIs.

---

## 🚀 Project Overview

This API allows users to:

* ➕ Create tasks
* 📖 Read all tasks or a single task
* ✏️ Update tasks
* ❌ Delete tasks

All data is stored **in memory** (no database), making it simple and perfect for learning and demos.

---

## 🧠 Why This Project Matters

In real-world AI/ML systems:

* Models are served via **web APIs**
* FastAPI is widely used for **model inference services**
* Pydantic ensures **safe & validated inputs**

This project builds the **foundation** needed for deploying ML models later.

---

## 🛠 Tech Stack

* **Python 3.10+**
* **FastAPI** – API framework
* **Uvicorn** – ASGI server
* **Pydantic** – Data validation

---

## 📂 Project Structure

```text
FastApi_CRUD/
│
├── main.py        # FastAPI app & routes
├── schemas.py    # Pydantic models (request/response)
├── data.py       # In-memory data storage
├── venv/         # Virtual environment
└── README.md     # Project documentation
```

---

## ⚙️ Setup Instructions (Windows)

### 1️⃣ Clone or Create Project Folder

```bash
mkdir FastApi_CRUD
cd FastApi_CRUD
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

### 3️⃣ Activate Virtual Environment

```bash
venv\Scripts\Activate
```

You should see:

```text
(venv)
```

### 4️⃣ Install Dependencies

```bash
pip install fastapi uvicorn
```

---

## ▶️ Run the Application

From inside the `FastApi_CRUD` folder:

```bash
python -m uvicorn main:app --reload
```

Server will start at:

```text
http://127.0.0.1:8000
```

---

## 📘 API Documentation (Swagger UI)

FastAPI provides automatic interactive documentation.

Open in browser:

```text
http://127.0.0.1:8000/docs
```

You can test **all CRUD operations directly from the browser**.

---

## 🔁 CRUD API Endpoints

### ➕ Create Task

**POST** `/tasks`

Request Body:

```json
{
  "title": "Learn FastAPI",
  "description": "Practice CRUD operations"
}
```

---

### 📖 Get All Tasks

**GET** `/tasks`

---

### 🔍 Get Task by ID

**GET** `/tasks/{task_id}`

---

### ✏️ Update Task

**PUT** `/tasks/{task_id}`

Request Body:

```json
{
  "title": "Learn FastAPI Deeply",
  "description": "CRUD + Validation"
}
```

---

### ❌ Delete Task

**DELETE** `/tasks/{task_id}`

---

## ❗ Error Handling

If a task does not exist:

* Status Code: **404 Not Found**
* Response:

```json
{
  "detail": "Task not found"
}
```

---

## 🧩 Key Concepts Covered

* HTTP methods (GET, POST, PUT, DELETE)
* REST API principles
* FastAPI routing
* Path & request body parameters
* Pydantic schema validation
* In-memory data storage
* Error handling with HTTPException
* Auto-generated API documentation

---

## 🧪 Testing Options

* ✅ Swagger UI (`/docs`)
* ✅ Postman
* ✅ Curl commands

---

## 🚀 Future Enhancements

* Add task completion toggle
* Use a database (SQLite / PostgreSQL)
* Add authentication (JWT)
* Convert into ML model inference API
* Dockerize the application

---

---

✨ *Built with FastAPI to learn modern API development*
