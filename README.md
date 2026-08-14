#  Cloud Notes Keeper

A simple cloud computing mini-project — a note-taking web application built with **Flask** (Python) and deployed on **Render** (Platform-as-a-Service / PaaS).

## Cloud Computing Concepts Demonstrated
- **Platform as a Service (PaaS):** The app is deployed on Render, which manages the underlying servers, OS, and runtime — the developer only manages application code.
- **Scalability:** Render can scale the web service (dyno/instance) up or down based on traffic.
- **Cloud Database Storage:** Notes are stored persistently and accessed over the web instead of locally on a device.
- **On-demand accessibility:** The app is accessible from anywhere via a public URL, demonstrating the "broad network access" characteristic of cloud computing (NIST cloud definition).

## Tech Stack
- Backend: Python, Flask
- Database: SQLite
- Deployment: Render (Cloud PaaS)
- Frontend: HTML, CSS (Jinja2 templates)

## Features
- Add notes (title + content)
- View all saved notes
- Delete notes
- Data persists across sessions (stored server-side in the cloud)

## How to Run Locally
```bash
pip install -r requirements.txt
python app.py
```
Visit `http://localhost:5000`

## Deployment (Render)
1. Push this project to GitHub.
2. Go to render.com → New → Web Service.
3. Connect your GitHub repo.
4. Build Command: `pip install -r requirements.txt`
5. Start Command: `gunicorn app:app`
6. Deploy — Render gives a live public URL.
