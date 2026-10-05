# My To-Do List

A simple Flask web application for adding tasks and tracking whether they are complete. This coursework project demonstrates how Python routes, HTML forms, and templates work together.

## Features

- Add a task through the web form.
- Mark a task complete or incomplete.
- Display an empty-list message before tasks are added.
- Change the task's completion styling through CSS classes.

## Technologies

Python, Flask 2.3.3, Werkzeug 2.3.7, HTML, CSS, and Flask's Jinja templates.

## Project structure

- `app.py`: Flask routes and in-memory task list.
- `requirements.txt`: Python dependencies.
- `templates/index.html`: Task input and task list.
- `static/style.css`: Page styling.
- [REFLECTION.md](REFLECTION.md): Development reflection.

## Run locally

Enter these commands in a terminal:

```bash
git clone https://github.com/kentrelpeters/todo-app.git
cd todo-app
python3 -m venv venv
```

On macOS or Linux, activate the environment:

```bash
source venv/bin/activate
```

On Windows Command Prompt, use `python` instead of `python3` when creating the environment, then activate it:

```bat
venv\Scripts\activate
```

Install the dependencies and start the app:

```bash
python -m pip install -r requirements.txt
python app.py
```

Open http://127.0.0.1:5000 in your browser. To stop the server, press **Ctrl+C** in the terminal.

## Usage example

1. Enter `Review Python notes` and click **Add Task**.
2. Click **Mark as Complete** beside the task.
3. Click **Mark as Incomplete** to switch it back.

These steps provide a manual check of the main task flow.

## Limitations

Tasks are stored in a Python list in server memory. Restarting the server clears the list, and visitors to the same server share it. The app does not include accounts, a database, or task deletion. It runs with Flask debug mode enabled for local development.

## Possible next improvements

Add persistent storage, task deletion, and automated checks for the task routes.
