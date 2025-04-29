
---

# 📦 Backend README

# 🎓 Graduación - Backend

This folder contains the **Django REST API** for the Graduacion project.

---

## 🚀 Quickstart

1. Create and activate a virtual environment:

```bash
uv venv
source .venv/bin/activate
```

2. Install the project dependencies:

```bash
uv sync pyproject.toml
```
3. Apply migrations:

```bash
uv python manage.py migrate
```

4. Run the development server:

```bash
uv python manage.py runserver
```

The backend will be available at http://localhost:8000/.

---

## ⚙️ Environment Variables

Create a .env file in the backend/ folder with the following (example):

```bash
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgres://username:password@localhost:5432/graduacion
```

---

## 🧪 Testing

To run backend tests:

```bash
uv python manage.py test
```

---

## 📚 Documentation

To generate documentation:

```bash
uv python manage.py generate_docs
```

The documentation will be available at http://localhost:8000/docs/.

---

## 🧱 Stack

- Django 5
- Django REST Framework
- PostgreSQL
- uv (dependency management)
