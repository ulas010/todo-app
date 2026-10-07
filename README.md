# To-Do List (frontend)

A task manager built with plain HTML, CSS and JavaScript. The frontend talks to a REST API to create, read, update and delete tasks. I built it during my internship at Softalya Software (July–August 2024) in a two-person team: I wrote the frontend, a teammate wrote the backend.

## Features

- Add a task with a title and a description
- Edit a task
- Delete a task
- Click a task to mark it as completed (or not)
- Tasks are loaded from the backend when the page opens

## Tech

- HTML5, CSS3
- JavaScript (Fetch API, async/await, DOM manipulation)
- REST API calls: `GET`, `POST`, `PATCH`, `DELETE`

## Run it

Open `index.html` in a browser.

- **Without a backend:** the app switches to *demo mode* automatically and saves tasks in your browser's `localStorage`. A notice at the top tells you when this happens.
- **With a backend:** set `API_URL` at the top of the script in `index.html`. The API is expected to provide:

| Method | URL | Purpose |
| --- | --- | --- |
| GET | `/todo/` | list all tasks |
| POST | `/todo/` | create a task (`title`, `description`, `completed`) |
| PATCH | `/todo/<id>/` | update a task |
| DELETE | `/todo/<id>/` | delete a task |

## Notes

The demo mode fallback was added after the internship so the project can be tried without running the backend.
