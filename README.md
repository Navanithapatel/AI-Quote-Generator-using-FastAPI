# FastAPI Project – Setup & Run Guide

## Project Overview

This project is a **FastAPI-based backend application**.
It uses a **virtual environment**, installs dependencies from `requirements.txt`,
runs the server using **Uvicorn**, and APIs can be tested with **Thunder Client** in VS Code.

---

## Step-by-Step Setup

### 1. Open Project Folder

```bash
cd "your_project_folder"
```

---

### 2. Create Virtual Environment

```bash
python -m venv venv
```

---

### 3. Activate Virtual Environment

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

---

### 4. Install Required Packages

```bash
pip install -r requirements.txt
```

---

## Run the FastAPI Server

```bash
uvicorn main:app --reload
```

* `main` → Python file name (`main.py`)
* `app` → FastAPI instance inside the file
* `--reload` → Auto-restart server on code changes

After running, open in browser:

```
http://127.0.0.1:8000
```

---

## API Testing Using Thunder Client

1. Install **Thunder Client** extension in VS Code.
2. Open Thunder Client panel.
3. Create a **New Request**.
4. Enter API URL (example):

   ```
   http://127.0.0.1:8000/docs
   ```
5. Choose method (**GET / POST / PUT / DELETE**) and send request.

---

## Important Notes

* Do **not upload** `venv/` or `.env` to GitHub.
* Always include **requirements.txt**.
* Ensure Python is installed and added to **PATH**.

---

## Purpose of the Project

To build and test **REST APIs using FastAPI**,
run them locally with **Uvicorn**, and verify endpoints using **Thunder Client**.

---

## Author

Created for **learning and academic practice**.
