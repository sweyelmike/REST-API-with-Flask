# 🚀 Flask User Management REST API

A simple, lightweight RESTful API built with Flask demonstrating full CRUD (Create, Read, Update, Delete) capabilities using in-memory storage.

| Badge | Status |
| :--- | :--- |
| ![Python Version](https://img.shields.io/badge/Python-3.x-blue.svg) | Python 3 |
| ![Framework](https://img.shields.io/badge/Framework-Flask-black.svg) | Flask |
| ![Style](https://img.shields.io/badge/Style-RESTful-orange.svg) | REST API |

---

## ✨ Features & Endpoints

This application exposes four primary endpoints for managing user data:

| Method | Route | Description | HTTP Status |
| :--- | :--- | :--- | :--- |
| `GET` | `/users` | Retrieve all users. | 200 OK |
| `POST` | `/users` | Add a new user. | 201 Created |
| `PUT` | `/users/<int:user_id>` | Update an existing user by index. | 200 OK / 404 Not Found |
| `DELETE` | `/users/<int:user_id>` | Remove a user by index. | 200 OK / 404 Not Found |

> **Note:** Data is stored in a simple Python list (`users = []`) and is reset every time the server stops.

---

## 🛠️ Tech Stack & Requirements

* **Language:** Python 3
* **Web Framework:** Flask
* **Tools:** VS Code, cURL (for testing)

---

## ⚙️ Installation & Setup

1.  **Clone or Create the Project Directory:**
    ```bash
    mkdir flask_api
    cd flask_api
    ```

2.  **Create and Activate Virtual Environment:**
    ```bash
    python -m venv venv
    # Linux/Mac: source venv/bin/activate
    # Windows: venv\Scripts\activate
    ```

3.  **Install Dependencies:**
    The `requirements.txt` should contain just `flask`.
    ```bash
    pip install -r requirements.txt
    # OR: pip install flask
    ```

---

## ▶️ Running the Application

Execute the main file within your activated environment:

```bash
python app.py
