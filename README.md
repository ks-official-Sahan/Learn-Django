# Learn Django

Django is a high-level Python web framework that encourages rapid development and clean, pragmatic design. This repository is dedicated to learning Django by building a sample application from scratch. The project covers installation, setup, basic app creation, and best practices.

---

## Table of Contents

- [Learn Django](#learn-django)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
  - [Overview](#overview)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
    - [Python Installation](#python-installation)
    - [Django Installation](#django-installation)
  - [Project Setup](#project-setup)
  - [Running the Application](#running-the-application)
  - [Project Structure](#project-structure)
  - [Contributing](#contributing)
  - [License](#license)
  - [Additional Resources](#additional-resources)

---

## Getting Started

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/ks-official-sahan/Learn-Django.git
   cd Learn-Django
   ```

2. **Set Up the Virtual Environment:**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Development Server:**

   ```bash
   python manage.py runserver
   ```

---

## Overview

This project serves as a starting point for learning Django. It demonstrates the fundamentals of creating a Django project, setting up an application, and running the development server. As you progress, you can extend the project with additional apps, features, and integrations.

---

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Python 3.13 or higher (preferably installed using the official [Python Download](https://www.python.org/downloads/))
- Git (for version control)
- A code editor (e.g., VS Code, PyCharm)

---

## Installation

### Python Installation

Download and install Python from the official [Python Download](https://www.python.org/downloads/) page.

_Or (For Windows users using Winget):_

```yaml
winget install --id Python.Python.3.13 --source winget
```

### Django Installation

1. **Upgrade pip and Install Django**  
   Open your terminal or command prompt and run:

```yaml
py -m ensurepip --upgrade
python -m pip install --upgrade pip
py -m pip install django
```

2. **Verify Installation**  
   Check the installed Django version:

```yaml
python -m django --version
```

---

## Project Setup

1. **Create a Project Directory**

```yaml
mkdir project_folder cd project_folder
```

2. **Create a Django Project**

```yaml
django-admin startproject project_name .
```

3. **Apply Project Migrations**

```yaml
py manage.py migrate
```

4. **Create Your First App (e.g., Polls)**

```yaml
py manage.py startapp polls
```

_Note: Remember to add `'polls'` to the `INSTALLED_APPS` list in `project_name/settings.py`._

---

## Running the Application

Start the Django development server with one of the following commands:

- **Default Port (8000):**

```yaml
py manage.py runserver
```

- **Custom Port (e.g., 1500):**

```yaml
py manage.py runserver 1500
```

- **Custom IP and Port:**

```yaml
py manage.py runserver 1.2.3.4:7000
```

Visit `http://127.0.0.1:8000/` (or the appropriate address) in your browser to see the app in action.

---

## Project Structure

A recommended structure for this project:

```yaml
Learn-Django/
├── docs/                   # Documentation and learning notes
├── project_name/           # Django project core files (settings, URLs, wsgi)
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── polls/                  # Sample app (e.g., polls) with models, views, templates
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── tests/                  # Additional test scripts
├── .gitignore              # Git ignore rules (e.g., virtual environment, __pycache__)
├── README.md               # This file
└── LICENSE                 # Licensing information (MIT License)
```

---

## Contributing

Contributions are welcome! If you’d like to improve this project or add new features, please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:

```yaml
git checkout -b feature/your-feature-name
```

3. Commit your changes with clear, descriptive messages.
4. Push to your fork and submit a pull request.
5. Follow the repository's coding conventions and write tests where applicable.

For detailed guidelines, see the CONTRIBUTING.md file if available.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Additional Resources

- [Django Official Documentation](https://docs.djangoproject.com/en/stable/)
- [Django Tutorial: Writing your first Django app](https://docs.djangoproject.com/en/stable/intro/tutorial01/)
- [Python Official Documentation](https://docs.python.org/3/)

---

Happy coding and enjoy your Django journey!
