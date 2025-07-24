
# 🌐 Django Starter with UV (UltraViolet)

This is a beginner-friendly guide to getting started with **Django** using **UV**, a super-fast Python package manager written in Rust. This project setup helps you build Django applications quickly and efficiently.

---

## 📦 What is UV?

**UV** is a fast Python package manager and virtual environment tool, designed to replace `pip`, `venv`, and `virtualenv` — all in one.

🔗 Official site: [https://astral.sh/blog/posts/introducing-uv/](https://astral.sh/blog/posts/introducing-uv/)

---

## ✅ Prerequisites

Before you begin:

- Python 3.7 or higher installed
- Git (optional, for cloning projects)
- Terminal / Command prompt access

---

## ⚙️ Installation

### 📥 Install UV

**Option 1: Curl (recommended)**

```bash
curl -Ls https://astral.sh/uv/install.sh | sh
```

**Option 2: Homebrew (macOS/Linux)**

```bash
brew install astral-sh/uv/uv
```

### 🔍 Check installation

```bash
uv --version
```

---

## 🚀 Getting Started with Django

Follow these steps to create a Django project using UV:

---

### 1. 📁 Create a Project Directory

```bash
mkdir my_django_project
cd my_django_project
```

---

### 2. 🔒 Create and Activate Virtual Environment

```bash
uv .venv
```

**Activate it:**

- **Linux/macOS:**
  ```bash
  source .venv/bin/activate
  ```
- **Windows (cmd):**
  ```cmd
  .venv\Scripts\activate.bat
  ```
- **Windows (PowerShell):**
  ```powershell
  .venv\Scripts\Activate.ps1
  ```

---

### 3. 📦 Install Django

```bash
uv pip install django
```

---

### 4. 📁 Create a Django Project

```bash
django-admin startproject core .
```

The dot `.` puts files in the current directory instead of a subfolder.

---

### 5. 🚀 Run the Development Server

```bash
python manage.py runserver
```

Then visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

### 6. 📜 Freeze Your Requirements

```bash
uv pip freeze > requirements.txt
```

---

### 7. 🔁 Install From Requirements (later)

```bash
uv pip install -r requirements.txt
```

---

## 🔧 Common Django Commands

| Task                          | Command                       |
|-------------------------------|-------------------------------|
| Create project                | `django-admin startproject`   |
| Run development server        | `python manage.py runserver`  |
| Make new app                  | `python manage.py startapp`   |
| Make migrations               | `python manage.py makemigrations` |
| Apply migrations              | `python manage.py migrate`    |
| Create superuser              | `python manage.py createsuperuser` |
| Collect static files          | `python manage.py collectstatic` |

---

## 📁 Project Structure (after setup)

```
my_django_project/
├── .venv/
├── manage.py
├── core/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── requirements.txt
```

---

## 📝 Notes

- Always activate your virtual environment before running any Django command.
- Use `uv pip` instead of `pip` to install packages.
- You can also add other packages like `djangorestframework`, `Pillow`, etc., the same way.

---

## 🙋‍♀️ Need Help?

- Django Docs: [https://docs.djangoproject.com](https://docs.djangoproject.com)
- UV GitHub: [https://github.com/astral-sh/uv](https://github.com/astral-sh/uv)

---

## 📌 License

This project is free to use and modify for educational or personal use.

---

## 🎉 Happy Coding with Django + UV!
