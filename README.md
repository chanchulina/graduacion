# 🎓 Graduacion Project

**Graduacion** is a web-based system for a to-do list, developed to use my knowledge in programming.

This repository is a **monorepo** containing:

- 📦 **Backend**: REST API built with Django.
- 🎨 **Frontend**: Web application built with React (Vite + Tailwind CSS).

---

## 📂 Project Structure

graduacion/
├── backend/                   # Django API
│   ├── .venv/                # Virtual environment for backend dependencies (do not commit to Git)
│   ├── .python-version       # Python version used by uv for backend
│   ├── manage.py               # Entry point for backend
│   ├── pyproject.toml        # Project dependencies and metadata
│   ├── app/
│   ├── uv.lock               # Lock file for uv dependencies
│   └── README.md
│
├── frontend/            # React Application
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── README.md
│
├── docker-compose.yml   # (optional)
├── Makefile             # (optional)
└── README.md            # Root project documentation



---

## ⚠️ Important Notes

- `.venv/` is the virtual environment created by `uv`. **It should not be committed to Git**. Make sure `.venv/` is listed in `.gitignore`.
- `.python-version` specifies the Python version used for the project (e.g., `3.12`). It helps `uv` or tools like `pyenv` manage the correct Python version automatically.
- `pyproject.toml` is the primary file where project dependencies and metadata are declared.
- `uv.lock` locks the exact versions of installed dependencies. It should be committed to ensure consistency across environments.
- If a `main.py` file was created automatically, but you are using Django, you can safely **delete it**. Django uses its own `manage.py` file for project management.

---

## 🚀 Quickstart

### Backend

```bash
cd backend
uv venv
source .venv/bin/activate
uv pip sync pyproject.toml
python manage.py migrate
python manage.py runserver
```
Backend will be running at http://localhost:8000/.

### Frontend

```bash
cd frontend
npm install
npm run dev
```
Frontend will be running at http://localhost:5173/.

---

## 🧱 Technologies

Area | Stack
Backend | Django, Django REST Framework, PostgreSQL
Frontend | React, Vite, Tailwind CSS
Tools | uv (Python dependency manager)

---

## ✍️ Authors

- **Maria Ignacia Strobel(https://github.com/chanchulina)** - *Software Engineer* - [Graduacion](https://github.com/chanchulina/Graduacion)
- **Jose Ignacio Schafer(https://github.com/kadkeno)** - *Tech lead* - [Graduacion](https://github.com/kadkeno/Graduacion)

---

# 🎯 Resumen

| Archivo            | Contenido                                                  |
|---------------------|-------------------------------------------------------------|
| `graduacion/README.md` | General overview of the whole monorepo |
| `graduacion/backend/README.md` | Instructions for the Django backend |
| `graduacion/frontend/README.md` | Instructions for the React frontend |
