# Django Demo Application

A basic Django web application template with a clean structure and essential configurations.

## Features

- Django 5.2.1
- SQLite database (default)
- Custom user model ready
- Static files configured
- Bootstrap-ready templates
- Admin interface

## Prerequisites

- Python 3.8+
- pip (Python package manager)

## Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd BlackcofferDjango
   ```

2. **Set up a virtual environment**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - On Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run migrations**
   ```bash
   python manage.py migrate
   ```

6. **Create a superuser (admin account)**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server**
   ```bash
   python manage.py runserver
   ```

8. **Access the application**
   - Main site: http://127.0.0.1:8000/
   - Admin interface: http://127.0.0.1:8000/admin/

## Project Structure

```
BlackcofferDjango/
├── config/               # Project configuration
├── core/                 # Main application
│   ├── migrations/       # Database migrations
│   ├── templates/        # Application templates
│   ├── __init__.py
│   ├── admin.py         # Admin interface configuration
│   ├── apps.py          # Application configuration
│   ├── models.py        # Database models
│   ├── tests.py         # Test cases
│   ├── urls.py          # URL routing
│   └── views.py         # View functions
├── templates/            # Global templates
│   ├── base.html        # Base template
│   └── home.html        # Home page
├── .gitignore           # Git ignore file
├── manage.py            # Django management script
└── requirements.txt     # Project dependencies
```

## Development

- To create a new app:
  ```bash
  python manage.py startapp app_name
  ```

- To create and apply migrations:
  ```bash
  python manage.py makemigrations
  python manage.py migrate
  ```

## License

This project is open source and available under the [MIT License](LICENSE).
