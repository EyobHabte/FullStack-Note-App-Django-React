# FullStack Note App

**Full-stack Note-Taking Application** — React · Django · PostgreSQL

> A simple note-taking app with user authentication and full CRUD functionality for managing personal notes.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Repository Structure](#repository-structure)
5. [Prerequisites](#prerequisites)
6. [Installation](#installation)
7. [Usage](#usage)
8. [Running Tests](#running-tests)
9. [License](#license)

---

## Project Overview
FullStack Note App is a web-based application that allows users to create, read, update, and delete personal notes. It combines a React frontend with a Django REST API backend, persisting data in a PostgreSQL database.

## Features
- **User Authentication**: Sign up, log in, and secure session management.
- **CRUD Notes**: Create, view, edit, and delete notes.
- **Responsive UI**: Mobile-friendly interface with React.
- **REST API**: Backend APIs secured with JWT tokens.

## Tech Stack
- **Frontend**: React, React Router, Axios
- **Backend**: Django, Django REST Framework, JWT Authentication
- **Database**: PostgreSQL
- **Environment Management**: Python `venv`, npm

## Repository Structure
```plaintext
/                          # Project root
├── backend/               # Django project
│   ├── manage.py
│   ├── requirements.txt
│   └── <apps>/            # auth, notes
│       ├── migrations/
│       └── views.py
├── frontend/              # React application
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── README.md          # Frontend instructions
├── .gitignore
└── README.md              # This file
```

## Prerequisites
- Python 3.10+  
- Node.js 16+ & npm  
- PostgreSQL  
- Git  

## Installation

### 1. Clone the repo
```bash
git clone https://github.com/EyobHabte/FullStack-Note-App-Django-React.git
cd FullStack-Note-App-Django-React
```

### 2. Setup Backend
```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
# Edit database settings in settings.py
python manage.py migrate
python manage.py runserver
```

### 3. Setup Frontend
```bash
cd frontend
npm install
npm start
```

## Usage
- Open your browser at `http://localhost:3000` for the frontend.  
- The backend REST API runs at `http://localhost:8000/api/`.

## Running Tests
### Backend
```bash
cd backend
pytest
```

### Frontend
```bash
cd frontend
npm test
```

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

