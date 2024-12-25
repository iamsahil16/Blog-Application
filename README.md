# FastAPI with MySQL Integration

This project demonstrates how to use FastAPI to build a RESTful API with a MySQL database backend. The application includes routes for user management and post creation, retrieval, and deletion. Passwords are securely hashed using bcrypt.

## Features

- User authentication with secure password hashing.
- CRUD operations for posts.
- MySQL integration using SQLAlchemy.
- Lightweight, fast, and asynchronous framework with FastAPI.

## Prerequisites

Ensure the following are installed on your system:

- Python 3.7+
- MySQL Server
- Conda (or a preferred Python package manager)

  
## Project Structure

```plaintext
.
├── main.py           # Entry point of the application
├── models.py         # SQLAlchemy models for User and Post
├── database.py       # Database connection setup
├── requirements.txt  # Dependencies
├── README.md         # Documentation
```

## Database Models

### User Model

- **Fields:**
  - `id` (Primary Key)
  - `username`
  - `password` (hashed)

### Post Model

- **Fields:**
  - `id` (Primary Key)
  - `title`
  - `content`
  - `user_id` (Foreign Key to User)

