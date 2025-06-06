﻿# 📇 Contacts Web App
A simple full-stack contact management system built with Flask (Python) for the backend and React for the frontend. The app allows users to create, view, update, and delete contacts.


## 🔧 Tech Stack
### Backend (Flask)
Flask\
Flask-CORS\
Flask-SQLAlchemy\
SQLite (for local development)

### Frontend (React)
React 18+\
Fetch API\
CSS

## 🖥️ Backend Setup (Python + Flask)
### Prerequisites:
Python 3.x\
pip package manager
### Install Dependencies
```
cd backend
pip install Flask Flask-CORS Flask-SQLAlchemy
```
### Run the Flask App
```
python main.py
```
> [ By default, the server runs at: http://127.0.0.1:5000 ]

## 🌐 Frontend Setup (React)
### Prerequisites:
```
Node.js & npm
```
### Install and Run
```
cd frontend
npm install
npm run dev
```
> [ React app runs at: http://localhost:5173 (or your default Vite port) ]


## 📌 Features
✅ Create new contact\
📋 View list of all contacts\
✏️ Edit existing contact\
🗑️ Delete a contact


## ⚙️ API Endpoints (Flask)
| Method | Endpoint               | Description                |
| ------ | ---------------------- | -------------------------- |
| GET    | `/contacts`            | Get all contacts           |
| POST   | `/create_contact`      | Create a new contact       |
| PATCH  | `/update_contact/<id>` | Update an existing contact |
| DELETE | `/delete_contact/<id>` | Delete a contact           |


## Sample JSON Payload (POST/PATCH)
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}


## 🗃️ Database
Uses SQLite for lightweight local storage. The database file pyjsdatabase.db is created automatically on first run.


## 🔄 How Data Flows
React makes an HTTP request to Flask API.\
Flask processes and interacts with the SQLite database.\
The response is returned and reflected in the UI.

## 🧪 Sample Demo
Once both servers are running:\
Open http://localhost:5173\
Use the form to create a new contact\
The table will auto-refresh with new contact\
Click "Update" or "Delete" to manage contact


