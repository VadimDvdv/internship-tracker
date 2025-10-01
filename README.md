# Internship Tracker

A minimal web app to track internship applications, statuses, notes, and deadlines.

## Tech

- Backend: FastAPI (Python 3.12) or Flask (choose one)
- DB: SQLite (SQLAlchemy)
- Auth: session cookie (simple), upgradeable later
- Tests: pytest + coverage
- Deploy: Render/Fly/Railway (free tier)

## Features (v1)

- Companies CRUD
- Applications CRUD (company, role, location, link, status, notes, next action date)
- Filters: by status, by next action date
- CSV export (applications)
- Simple web UI (vanilla JS or small React page) that calls the API

## Getting Started

```bash
# one-time
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# run
uvicorn app.main:app --reload  # FastAPI
# or
flask --app app.main run --debug  # Flask
