# Task Management System

## Introduction
This project is a task management system where users can manage their tasks efficiently. The system allows users to create, view, edit, complete, and delete tasks. The data is persisted using MongoDB, and user-specific task management is implemented with a login and registration system. The frontend is built using Vite React.js for a fast and responsive user experience.


## Demo

Demo_Link: (https://drive.google.com/file/d/1PHI4W-QXX6iQaNajOhIvcDX801joe1PG/view?usp=sharing)

## Features

### Task Management
- **Create Tasks**: Users can create tasks with a title and description.
- **View Tasks**: Users can view a list of all their tasks.
- **Mark Tasks as Completed**: Users can mark tasks as completed.
- **Edit Tasks**: Users can edit task details.
- **Delete Tasks**: Users can delete tasks.

### User Management
- **User Registration**: New users can register to use the task management system.
- **User Login**: Registered users can log in to manage their tasks.

### Data Persistence
- Tasks are stored and retrieved from a MongoDB database to ensure data persistence.

### Validation and Error Handling
- Task titles must not be empty.
- Users cannot mark a task as complete if it is already marked as such.
- Errors are handled gracefully, with meaningful error messages provided to users.

## Technology Stack
- **Backend**: Node.js, Express.js
- **Frontend**: Vite, React.js
- **Database**: MongoDB

## Setup Instructions

### Prerequisites
- Node.js installed on your machine
- MongoDB installed and running

### Installation

1. **Clone the Repository**
    ```sh
   git clone https://github.com/rutxyz/Task_Management_Project-Node.git
   cd Task_Management_Project-Node

    ```

2. **Install Backend Dependencies**
    ```sh
    cd backend
    npm install
    ```

3. **Install Frontend Dependencies**
    ```sh
    cd ../frontend
    npm install
    ```

### Configuration

1. **Backend Configuration**
    - Create a `.env` file in the `backend` directory with the following content:
      ```env
       MONGO_URI=mongodb+srv://<username>:<password>@cluster0.htokwcl.mongodb.net/
       PORT=4000
       JWT_SECRET_KEY=sbfhdfhgdhgfhdgfhgdhfghsdgf
       JWT_EXPIRES=1000d
       COOKIE_EXPIRE=1000
       FRONTEND_URL=http://localhost:5173/

      CLOUDINARY_CLIENT_NAME=client_name here
      CLOUDINARY_CLIENT_API=<>
      CLOUDINARY_CLIENT_SECRET=<>

      ```

2. **Frontend Configuration**
    - Update the API base URL if necessary in the `frontend/src/config.js` file:
      ```js
      export const API_BASE_URL = 'http://localhost:4000/api';
      ```

### Running the Project

1. **Run the Backend**
    ```sh
    cd backend
    npm start
    ```

    The backend server will start on `http://localhost:4000`.

2. **Run the Frontend**
    ```sh
    cd ../frontend
    npm run dev
    ```

    The frontend development server will start, and you can view the application at `http://localhost:5173`.

### Usage

1. **Register a New User**
    - Navigate to the registration page and create a new user account.

2. **Login**
    - Log in with the registered user credentials.

3. **Manage Tasks**
    - Create, view, edit, complete, and delete tasks as needed.

## Error Handling and Validation

- Task titles are required and cannot be empty.
- A task cannot be marked as complete if it is already completed.
- Error messages are provided for validation failures and other errors.


## Contributing

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Push to the branch.
5. Create a pull request.

---

By following this documentation, you'll be able to set up, run, and understand the task management system, making a strong impression on interviewers with the organized and detailed structure of the project.
