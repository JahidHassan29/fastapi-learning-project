# FastAPI Learning Project

## Overview

This repository is a **beginner-friendly, professional FastAPI project** created to learn and demonstrate core API development concepts used in modern backend and AI systems.

The project focuses on **API fundamentals, request/response handling, and data validation**, without introducing unnecessary complexity such as databases, authentication, cloud deployment, or large ML models.

The goal is to build a **clean mental model of how FastAPI works**, using industry-aligned structure and best practices.

---

## Project Goals

This project is designed to help you:

* Understand what an API is and how client–server communication works
* Learn FastAPI fundamentals (routes, HTTP methods, parameters)
* Validate request and response data using Pydantic
* Structure a FastAPI project in a clean, scalable way
* Use automatic API documentation (`/docs`)

This repository is intentionally kept **simple and focused**.

---

## What This Project Does

The API provides basic endpoints to:

* Confirm the API is running
* Accept structured JSON input
* Validate data using schemas
* Return JSON responses

No database or external services are used.

---

## Project Structure

```
fastapi-learning-project/
├── app/
│   ├── __init__.py        # Marks app as a Python package
│   ├── main.py            # FastAPI application entry point
│   ├── routes.py          # API route definitions
│   └── schemas.py         # Request and response schemas
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
├── .gitignore             # Ignored files
└── LICENSE                # MIT License
```

### Folder Responsibilities

* **app/**: Contains all application logic
* **main.py**: Creates the FastAPI app and includes routes
* **routes.py**: Defines API endpoints
* **schemas.py**: Defines Pydantic models for validation

---

## Technologies Used

* **Python 3.9+**
* **FastAPI** – API framework
* **Uvicorn** – ASGI server
* **Pydantic** – Data validation

---

## How to Run the Project

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Start the development server

```bash
uvicorn app.main:app --reload
```

### 3. Open in browser

* API root: `http://127.0.0.1:8000`
* Interactive docs: `http://127.0.0.1:8000/docs`

---

## Example API Behavior

**Request** (JSON):

```json
{
  "message": "Hello API"
}
```

**Response** (JSON):

```json
{
  "status": "success",
  "message": "Hello API"
}
```

---

## Design Principles

* **Simplicity first**: Learn fundamentals before adding complexity
* **Schema-driven validation**: Define data expectations clearly
* **Separation of concerns**: Routes, schemas, and app setup are isolated
* **Readable code**: Prioritize clarity over cleverness

---

## What This Project Does NOT Include

* Databases
* Authentication
* Docker
* Cloud deployment
* Production configuration

These topics are intentionally excluded to maintain focus on **FastAPI fundamentals**.

---

## Intended Audience

This project is suitable for:

* Beginners learning FastAPI
* ML / AI engineers learning API basics
* Developers transitioning from notebooks to services

---

## License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it.

---

## Next Steps

Possible future extensions (optional):

* Add PUT and DELETE endpoints
* Improve error handling
* Add simple ML logic
* Dockerize the application

These enhancements should only be added **after mastering the basics**.

---

## Summary

This repository demonstrates a clean, minimal FastAPI project that emphasizes correctness, structure, and clarity. It is designed as a learning and reference project for building real-world APIs in a disciplined way.
