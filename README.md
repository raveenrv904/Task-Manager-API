## Node.js Task Manager Project

### Description

This Node.js project is a task manager application that allows users to perform CRUD (Create, Read, Update, Delete) operations on tasks. It utilizes Express.js for routing, MongoDB for data storage, and implements error handling for various scenarios.

### Project Structure

- **`Controller.js`**: Defines functions for handling different task-related operations like getting all tasks, creating tasks, retrieving a specific task, updating a task, and deleting a task.
- **`Routes.js`**: Defines the API routes using Express Router, connecting HTTP methods (GET, POST, PATCH, DELETE) to their respective controller functions.
- **`App.js`**: Main entry point of the application, sets up Express server, connects to MongoDB, and defines middleware for static files, JSON parsing, error handling, and routing.

### File Structure

```
├── controllers
│   └── tasks.js
├── db
│   └── connect.js
├── errors
│   └── custom-error.js
├── middleware
│   ├── async.js
│   ├── error-handler.js
│   └── not-found.js
├── models
│   └── Task.js
├── routes
│   └── Task.js
├── app.js
└── .env (Environment variables)
```

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <project_folder>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Define the following environment variables:
     ```
     PORT=<port_number>
     MONGO_URL=<mongodb_connection_url>
     ```
4. Start the application:
   ```bash
   npm start
   ```

### API Endpoints

- `GET /api/v1/tasks`: Fetch all tasks.
- `POST /api/v1/tasks`: Create a new task.
- `GET /api/v1/tasks/:id`: Get a specific task by ID.
- `PATCH /api/v1/tasks/:id`: Update a specific task by ID.
- `DELETE /api/v1/tasks/:id`: Delete a specific task by ID.

### Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JavaScript

### How to Use

1. Make API requests to perform CRUD operations on tasks using the provided endpoints.
2. Ensure proper error handling for cases like invalid requests, non-existing tasks, etc.
3. Customize or extend functionality as needed for your project requirements.

### Notes

- This README provides an overview of the project's structure, functionalities, and setup instructions.
- Feel free to enhance the project by adding features, implementing user authentication, or improving error handling.
- Always handle sensitive data securely and follow best practices for production deployment.

### Author

RAVEEN R V - raveenrv92@gmail.com

### License

This project is licensed under the [MIT License](LICENSE).
