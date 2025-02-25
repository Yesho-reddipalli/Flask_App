# Task Master

Task Master is a simple task management web application built with Flask and SQLAlchemy.

## Features

- Add new tasks
- Update existing tasks
- Delete tasks
- View all tasks

## Requirements

- Python 3.9 or higher
- Flask 3.1.0
- Flask-SQLAlchemy 3.1.1
- Gunicorn 23.0.0

## Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Create a virtual environment and activate it:
    ```sh
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up the database:
    ```sh
    flask shell
    >>> from app import db
    >>> db.create_all()
    >>> exit()
    ```

## Usage

1. Run the application:
    ```sh
    python app.py
    ```

2. Open your web browser and go to `http://127.0.0.1:5000`.

## Project Structure

- [app.py]: Main application file
- [requirements.txt]: List of dependencies
- [static]: Static files (CSS)
- [templates]: HTML templates

## Tools Used

### Flask
Flask is a lightweight WSGI web application framework in Python. It is designed with simplicity and flexibility in mind, making it easy to get started with web development. Flask provides the essential tools and features needed to build web applications, such as routing, request handling, and templating.

### Flask-SQLAlchemy
Flask-SQLAlchemy is an extension for Flask that adds support for SQLAlchemy, a SQL toolkit and Object-Relational Mapping (ORM) library for Python. It simplifies database interactions by allowing developers to work with Python objects instead of writing raw SQL queries. Flask-SQLAlchemy integrates seamlessly with Flask, making it easy to manage database models and perform CRUD operations.

### Gunicorn
Gunicorn (Green Unicorn) is a Python WSGI HTTP server for UNIX. It is a pre-fork worker model, meaning it forks multiple worker processes to handle requests. Gunicorn is commonly used to deploy Python web applications in production environments due to its performance, reliability, and ease of use.

