# Todo App Backend

This is the backend component of a Todo application built using Node.js, Express.js, and MongoDB. It provides API endpoints to perform CRUD operations on tasks and user authentication.

## Installation

To get started with the Todo App Backend, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd todo-app-backend
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Set up environment variables:**

    Create a `.env` file in the root directory and define the following variables:

    ```plaintext
    PORT=3000
    MONGO_URI=<your-mongodb-connection-string>
    JWT_SECRET=<your-jwt-secret>
    ```

    Replace `<your-mongodb-connection-string>` with your MongoDB connection string and `<your-jwt-secret>` with a secret key for JWT token generation.

4. **Start the server:**

    ```bash
    npm start
    ```

## API Endpoints

### Tasks

- **POST /api/tasks/new**: Create a new task.
- **GET /api/tasks/my-tasks**: Get all tasks belonging to the authenticated user.
- **PATCH /api/tasks/:id**: Update a task's description and completion status.
- **DELETE /api/tasks/:id**: Delete a task.

### Authentication

- **POST /api/auth/register**: Register a new user.
- **POST /api/auth/login**: Login with email and password.
- **GET /api/auth/my-profile**: Get user's profile information.
- **POST /api/auth/logout**: Logout and clear authentication token.

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- bcrypt
- JSON Web Tokens (JWT)

## Contributors

- John Doe (@johndoe)
- Jane Smith (@janesmith)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
