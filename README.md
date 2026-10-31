@"
# Task Manager API

A backend REST API where users can register, log in, and manage their own tasks.

## Tech Stack
- Node.js and Express
- MongoDB Atlas with Mongoose
- JWT authentication and bcrypt password hashing

## Features
- Register and login with secure passwords
- Create, read, update, and delete tasks
- Each user sees only their own tasks
- Filter tasks by status

## API Endpoints
| Method | Endpoint | Description |
|---|---|---|
| POST | /api/auth/register | Create an account |
| POST | /api/auth/login | Log in and get a token |
| GET | /api/tasks | List your tasks (optional ?status=pending) |
| POST | /api/tasks | Create a task |
| GET | /api/tasks/:id | Get one task |
| PUT | /api/tasks/:id | Update a task |
| DELETE | /api/tasks/:id | Delete a task |

Task routes need the header: Authorization: Bearer YOUR_TOKEN

## Run Locally
1. npm install
2. Create a .env file with PORT, MONGO_URI and JWT_SECRET
3. npm run dev
"@ | Set-Content README.md
