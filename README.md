# To-Do List App

A simple To-Do List web application with a Node.js/Express/MongoDB backend and a vanilla JavaScript frontend.

## Features

- Add new tasks
- Mark tasks as completed
- Delete tasks
- Tasks are stored in MongoDB
- Responsive and clean UI

## Project Structure

```
list/
  backend/
    package.json
    server.js
    models/
      task.js
    routes/
      tasks.js
  frontend/
    list.html
    script.js
    style.css
```

## Getting Started

### Backend

1. **Install dependencies:**
   ```sh
   cd list/backend
   npm install
   ```
2. **Start MongoDB** (make sure MongoDB is running locally).
3. **Run the server:**
   ```sh
   npm start
   ```
   The backend will run on `http://localhost:5000`.

### Frontend

Open `list/frontend/list.html` in your browser.  
Make sure the backend server is running for the app to work.

## API Endpoints

- `GET /api/tasks` - List all tasks
- `POST /api/tasks` - Add a new task (`{ title }`)
- `PUT /api/tasks/:id` - Update a task (`{ completed }`)
- `DELETE /api/tasks/:id` - Delete a task

## Dependencies

- [Express](https://expressjs.com/)
- [Mongoose](https://mongoosejs.com/)
- [CORS](https://www.npmjs.com/package/cors)
- [Nodemon](https://nodemon.io/) (dev)
