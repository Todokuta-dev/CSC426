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

## Run Locally

### 1. Install Python (if not installed)
Download from https://python.org — make sure to check "Add to PATH" during install.

### 2. Install dependencies
Open terminal in the project folder and run:
```bash
pip install -r requirements.txt
```

### 3. Start the server
```bash
python app.py
```

### 4. Open in browser
Go to: http://localhost:5000

---

## Deploy to Render (Free)

### Step 1 — Push to GitHub
1. Create a GitHub account at https://github.com
2. Create a new repository named `login-app`
3. Upload all project files to the repository

### Step 2 — Create Render account
1. Go to https://render.com and sign up (free)
2. Click **New +** → **Web Service**
3. Connect your GitHub account and select the `login-app` repo

### Step 3 — Configure the service
Fill in these settings:
- **Name:** login-app (or anything you like)
- **Runtime:** Python 3
- **Build Command:** `pip install -r requirements.txt`
- **Start Command:** `gunicorn app:app`

### Step 4 — Add environment variable
Under **Environment**, add:
- Key: `SECRET_KEY`
- Value: any random string (e.g. `myapp-secret-2024-xyz`)

### Step 5 — Deploy
Click **Create Web Service**. Render will build and deploy automatically.
Your live URL will be: `https://your-app-name.onrender.com`

---

## Submission
Submit both:
1. GitHub repository URL
2. Live deployed URL (from Render)
