# Circles

Circles is a collaborative team platform built with Flask that helps users create teams, communicate in real time, assign tasks, share files, and manage project activity in one place.

## Overview

The application is designed for small teams and project groups that need a simple, centralized workspace for collaboration. Users can sign up, create teams, invite members, chat with teammates, and manage tasks with deadlines and status tracking.

## Features

- User registration and login
- Team creation and membership management
- Real-time messaging with Socket.IO
- Task assignment and tracking
- File upload and download support
- Team member profile and account management
- SQLite-backed data storage for rapid local development

## Tech Stack

- Python
- Flask
- Flask-SocketIO
- Flask-SQLAlchemy
- Flask-Login
- Flask-WTF
- SQLite

## Project Structure

```text
.
├── app.py                  # Main Flask application and route definitions
├── forms.py                # WTForms form definitions
├── models.py               # Database models and schema
├── momentjs.py             # Moment.js integration for templates
├── requirements.txt        # Python dependencies
├── static/                 # CSS, JS, and static assets
├── templates/              # HTML templates for the app
├── database.db             # SQLite database generated at runtime
└── README.md               # Project documentation
```

## Prerequisites

- Python 3.8+
- pip
- Virtual environment tool such as `venv`

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/flask-chat-master.git
cd flask-chat-master
```

2. Create a virtual environment:

```bash
python -m venv venv
```

3. Activate the environment:

- On macOS/Linux:

```bash
source venv/bin/activate
```

- On Windows:

```bash
venv\Scripts\activate
```

4. Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Application

Start the application with:

```bash
python app.py
```

Then open the app in your browser at:

```text
http://localhost:5000
```

The SQLite database will be created automatically when the application starts for the first time.

## Usage

1. Sign up for an account.
2. Create or join a team.
3. Start conversations in the team chat.
4. Add tasks and assign them to team members.
5. Upload relevant files and manage team updates.

## Notes

This project is intended for local development and lightweight collaboration workflows. For production deployment, it is recommended to use a production-ready web server, environment variables for sensitive settings, and a more robust database setup.

## License

This project is provided as-is for educational and development use.
