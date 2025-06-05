# 📝 FastAPI Open Blog (Backend)

This is the **backend** of a simple open blog application built with **FastAPI**.

The application provides a foundational API to:
- Create and delete blog posts
- Upload images
- Fetch all blog posts

> 🔧 No authentication is included to keep the project focused on core FastAPI features.

---

## 🚀 Features

- 📄 Create posts with image, title, content, and author name
- 📥 Upload images for posts
- 📃 Retrieve all blog posts
- ❌ Delete existing posts
- 🗃️ SQLite used as the database

---

## 🧰 Tech Stack

- **Python 3.12**
- **FastAPI**
- **SQLAlchemy**
- **SQLite**
- **Pydantic**
- **Uvicorn**

---

## 📂 Project Structure

```
fastapi-open-blog-backend/
├── main.py                     # FastAPI app entry point
├── requirements.txt            # Python dependencies
├── routers/
│   ├── post.py                 # Route definitions
│   └── schemas.py              # Pydantic models
├── database/
│   ├── database.py             # Database session
│   ├── models.py               # SQLAlchemy models
│   └── db_post.py              # DB operation functions
├── uploads/                    # Uploaded images (created automatically)
└── .gitignore                  # Files to ignore in git
```

---

## ⚙️ Getting Started

### 🛠️ Installation & Setup

1. **Clone the repository**

```bash
git clone https://github.com/SaifulAbir/fastapi-blog.git
cd fastapi-blog
```

2. **Create and activate a virtual environment**

```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```

3. **Install the dependencies**

```bash
pip install -r requirements.txt
```

4. **Run the application**

```bash
uvicorn main:app --reload
```

5. **Access the interactive API docs**

[http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 🧪 API Endpoints

| Method | Endpoint     | Description             |
|--------|--------------|-------------------------|
| GET    | `/post/all`  | Retrieve all blog posts |
| POST   | `/post`      | Create a new blog post  |
| DELETE | `/post/{id}` | Delete a blog post      |
| POST   | `post/image` | Upload an image         |

---

## 🗃️ Database

The SQLite database will be automatically created on first run if it doesn't exist.

> 🔒 **Do not commit the `*.db` file to version control.**

---

## 🌐 Frontend

The frontend (built with React) is hosted in a **separate repository**:  
➡️ [fastapi-blog-web](https://github.com/<your-username>/fastapi-open-blog-frontend)

---
<!--
## 📚 Course

This project is part of the  
🎓 [Complete FastAPI Masterclass from Scratch](https://www.udemy.com/) on Udemy.

--- -->

## 🛡 License

MIT License – free to use and modify.
