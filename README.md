# Task Manager Web Application

A simple Django-based web application for managing personal tasks with user authentication, task CRUD operations, search/filter, and pagination.

## Features
- **User Authentication**: Register, login, and logout functionality.
- **Task Management**: Create, read, update, and delete tasks.
- **Task Listing**: View tasks with search (by title), filter (by status), and pagination.
- **Responsive UI**: Built with Bootstrap for a clean, mobile-friendly interface.

## Tech Stack
- **Backend**: Django (Python)
- **Database**: MySQL
- **Frontend**: HTML, CSS, Bootstrap

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure the Database**:
   ```SQL
   CREATE DATABASE taskmanager;
   ```
   Update TaskManagerProject/taskmanager/settings.py with your database credentials:
   ```python
   DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'taskmanager',
        'USER': 'your_username',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '3306',
      }
   }
   ```

5. **Apply Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Collect Static Files**:
   ```bash
   python manage.py collectstatic
   ```

6. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```
