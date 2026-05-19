# Submission Detail
---

# Technologies Used

- Python
- FastAPI
- SQLAlchemy
- MySQL
- Pydantic
- Uvicorn

---
---

# Features

- Category CRUD APIs
- Product CRUD APIs
- One-to-Many relationship between Category and Product
- Server-side pagination
- ORM implementation using SQLAlchemy
- Swagger API documentation

---


## GitHub Repo Link

Repo Link:
```bash
https://github.com/aman70216/AssingmentGivenByNimapInfotech
```

---

# Steps to Run the Application

## 1. Clone the Repository

```bash
git clone <your-github-repository-link>
```

---

## 2. Move to Project Directory

```bash
cd fastapi-crud-assignment
```

---

## 3. Create Virtual Environment Venv

```bash
python -m venv venv
```

---

## 4. Activate virtual environment enter the below command in terminal

### Windows

```bash
venv\Scripts\activate
```

---

## 5. Install required dependencies

```bash
pip install -r requirements.txt
```

---

# Database Configuration

Use Mysql and configure it By replacing Your root with Your User Name and 992Aman* with your Password

```python
DATABASE_URL = "mysql+pymysql://root:992Aman*@localhost/ProductAndCategory"
```

Create database in MySQL:

```sql
CREATE DATABASE ProductAndCategory;
```

---

# Server startup cmd

Run the FastAPI server using:

```bash
uvicorn app.main:app --reload
```

---

# Swagger api Documentation

After server starts successfully:

```bash
http://127.0.0.1:8000/docs
```

---

# Database design details

## Categories table

| Column Name | Data Type | Description |
|---|---|---|
| id | Integer | Primary Key |
| name | String | Category Name |

---

## Products Table

| Column Name | Data Type | Description |
|---|---|---|
| id | Integer | Primary Key |
| name | String | Product Name |
| price | Float | Product Price |
| category_id | Integer | Foreign Key referencing Categories table |

---

# Relationship

One Category can have multiple Products.

Each Product belongs to one Category.

Relationship Type:
```bash
One-to-Many
```
# Built by Aman Mishra 