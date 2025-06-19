# 🧠 FastAPI Blog Backend (SQLite Edition)

A lightweight, backend-only **Blog API** built with **FastAPI** and **SQLite**, focused on learning and backend logic.  
Includes full **CRUD**, **JWT authentication**, and clean modular structure—ready for future frontend integration.

---

## 📌 Features

✅ User Registration / Login (JWT)  
✅ Token-Based Authentication  
✅ Create / Read / Update / Delete Blog Posts  
✅ SQLite (no setup needed—just run)  
✅ Secure Password Hashing with PassLib  
✅ Modular and Clean File Structure

---

## 🛠️ Tech Stack

- **FastAPI** – modern Python web framework  
- **SQLite** – lightweight built-in database  
- **SQLAlchemy** – ORM for DB models  
- **Pydantic** – data validation  
- **Passlib** – password hashing  
- **Python-Jose** – JWT handling

---

## 📂 Folder Structure

.
├── app
│ ├── main.py # FastAPI app entry
│ ├── database.py # SQLite DB connection
│ ├── models.py # SQLAlchemy models
│ ├── schemas.py # Pydantic schemas
│ ├── hashing.py # Password hashing logic
│ ├── jwt_token.py # JWT token utilities
│ ├── oauth2.py # Dependency for auth
│ └── routers
│ ├── blog.py # Blog routes
│ └── user.py # User routes
├── requirements.txt
└── README.md

yaml
Copy
Edit

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/fastapi-blog-backend.git
cd fastapi-blog-backend
2. Set Up Environment
bash
Copy
Edit
# Create virtual environment
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
3. Run the Server
bash
Copy
Edit
uvicorn app.main:app --reload
🔐 Example API Endpoints
Endpoint	Method	Description
/register	POST	Register new user
/login	POST	Login and get token
/blogs	GET	Get all blogs (auth)
/blogs/{id}	GET	Get blog by ID (auth)
/blogs	POST	Create blog (auth)
/blogs/{id}	PUT	Update blog (auth)
/blogs/{id}	DELETE	Delete blog (auth)

Use Thunder Client or Postman to test the API locally.

💡 Why I Built This
This project was made to focus purely on backend logic using FastAPI with no distractions from frontend work.
I wanted a clean, working backend I could expand later—with Flutter, Next.js, or whatever else.

Even if you're learning and feel behind—this counts. This is real experience.

📋 Future Goals
Connect a frontend (maybe Flutter or Next.js)

Add comments, likes, tags

Role-based access (admin, users)

Deployment on Render or Railway

