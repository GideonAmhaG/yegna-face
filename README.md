# Yegnaface

Yegnaface is a social media application designed for Ethiopians to connect, share, and engage with each other. Built using React for the frontend and Node.js with Express for the backend, this application provides a seamless user experience with features like user authentication, posting, and friend management.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Available Scripts](#available-scripts)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and login
- Profile management
- Post creation and sharing
- Friend management (add/remove friends)
- Real-time updates on posts and comments
- Responsive design for mobile and desktop

## Technologies Used

- **Frontend:**
  - React
  - Redux for state management
  - Material-UI for UI components
  - Formik and Yup for form handling and validation
  - React Router for routing

- **Backend:**
  - Node.js
  - Express
  - MongoDB with Mongoose for database management
  - JWT for authentication
  - Multer for file uploads

## Getting Started

These instructions will help you set up the project locally for development and testing.

### Prerequisites

Make sure you have the following installed:

- Node.js (version >= 14.0.0)
- MongoDB (for local development)

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Navigate to the client directory:
   ```bash
   cd client
   ```

3. Install the frontend dependencies:
   ```bash
   npm install
   ```

4. Navigate to the server directory:
   ```bash
   cd ../server
   ```

5. Install the backend dependencies:
   ```bash
   npm install
   ```

6. Create a `.env` file in the server directory and add your MongoDB connection string:
   ```
   MONGO_URL=<your_mongodb_connection_string>
   PORT=6001
   ```

7. Start the backend server:
   ```bash
   npm run dev
   ```

8. In a new terminal, navigate back to the client directory and start the frontend:
   ```bash
   cd client
   npm start
   ```

## Available Scripts

In the client directory, you can run:

### `npm start`

Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

### `npm test`

Launches the test runner in interactive watch mode.

### `npm run build`

Builds the app for production to the `build` folder.

### In the server directory:

### `npm run dev`

Starts the server in development mode using Nodemon.

## API Endpoints

### Authentication

- **POST /auth/register**: Register a new user
- **POST /auth/login**: Log in an existing user

### Users

- **GET /users/:id**: Get user details
- **PATCH /users/:id/:friendId**: Add or remove a friend

### Posts

- **POST /posts**: Create a new post
- **GET /posts**: Get all posts
- **GET /posts/:userId/posts**: Get posts by a specific user
- **PATCH /posts/:id/like**: Like or unlike a post

## Contributing

If you would like to contribute to this project, please fork the repository and create a pull request. 

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.