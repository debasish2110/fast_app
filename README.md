# Tracker App — FastAPI + React

A simple **Tracker Application** built with **FastAPI** (backend) and **React** (frontend).  
This project is part of my learning journey with FastAPI and modern web development.

---

## 🚀 Tech Stack

**Frontend:** React, JavaScript, HTML, CSS  
**Backend:** FastAPI, Python  
**Others:** REST API, Axios (for API calls), Node.js, Uvicorn

---

## 📁 Project Structure

```
tracker-app/
│
├── backend/                     # FastAPI backend
|   ├── models
|   |   ├── product_models.py
|   |   └── __init__.py
│   ├── app.py                   # Entry point for FastAPI app
│   ├── requirements.txt         # Backend dependencies
│   └── DockerFile               
│
├── frontend/                    # React frontend
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── DockerFile
│
├── docker-compose.yaml
└── README.md
```

---

## ⚙️ Setup Instructions

### 🐍 Backend (FastAPI)

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r backend/requirements.txt
   ```

4. Run the FastAPI server:
   ```bash
   uvicorn app:app --reload
   ```

   The backend will start at:  
   👉 http://127.0.0.1:8000

---

**FOR SWAGGER IN FAST API, U CAN EXECUTE (inbuilt swagger docs): ```http://127.0.0.1:8000/docs```**

### ⚛️ Frontend (React)

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the React development server:
   ```bash
   npm start
   ```

   The frontend will run on:  
   👉 http://localhost:3000

---

## 🔗 Connecting Frontend & Backend

Ensure your frontend (React) calls the backend API endpoints correctly.  
For example, in your React code:

```javascript
axios.get("http://127.0.0.1:8000/api/tasks")
     .then(response => console.log(response.data))
     .catch(error => console.error(error));
```

You can also define the base API URL in a `.env` file inside your `frontend/` directory:
```
REACT_APP_API_BASE_URL=http://127.0.0.1:8000
```

---

## 🧠 Learning Goals

- Understand FastAPI’s routing, Pydantic models, and dependency injection  
- Build RESTful APIs and integrate them with a frontend  
- Manage state and API requests using React and Axios  
- Learn how to structure a full-stack project efficiently  

---

## 🧩 Possible Features (Tracker App Ideas)

You can use this setup to build:
- ✅ **Task Tracker** — Track daily tasks or goals  
- 💰 **Expense Tracker** — Record and analyze expenses  
- 🕒 **Habit Tracker** — Maintain and visualize progress over time  

---

## 🧰 Useful Commands Summary

| Purpose | Command |
|----------|----------|
| Install backend dependencies | `pip install -r requirements.txt` |
| Run FastAPI backend | `uvicorn main:app --reload` |
| Install frontend dependencies | `npm install` |
| Run React frontend | `npm start` |

---

## 📜 License

This project is for **learning purposes** only.  
Feel free to fork and modify it for your personal experiments.

---

## ✨ Author

**Debashish Dash**  
Learning FastAPI & React ⚡  
[LinkedIn](https://linkedin.com/in/debashish98)
