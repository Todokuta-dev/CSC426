# AuthApp — Flask Login System

A full-stack login/signup web app built with Python (Flask) + SQLite.

## Features
- User signup with hashed passwords (bcrypt)
- Login with username or email
- Session management
- Input validation on both frontend and backend
- Responsive glassmorphism UI
- Protected dashboard route

## Project Structure
```
login-app/
├── app.py                 ← Flask backend
├── requirements.txt       ← Python dependencies
├── Procfile               ← Render deploy config
└── templates/
    ├── login.html         ← Login/Signup page
    └── dashboard.html     ← Protected dashboard
```

---

