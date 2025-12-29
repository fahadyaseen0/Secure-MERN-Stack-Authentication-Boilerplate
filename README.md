# MERN Authentication and Protected Routes Project

This project demonstrates a basic MERN (MongoDB, Express, React, Node.js) stack application with JWT-based authentication and route protection. It includes features such as user registration, login, and protected routes. Additionally, it prevents logged-in users from accessing the login and registration pages.

## Features

- **User Authentication**: Users can register, log in, and receive a JWT token for authentication.
- **Protected Routes**: Certain routes are only accessible to authenticated users.
- **Public Routes**: Redirects authenticated users away from the login and registration pages.
- **React Router v6**: Utilizes the latest version of React Router for navigation.



## Project Structure

- **Backend (Node.js/Express)**: Handles user authentication, JWT token generation, and route protection.
- **Frontend (React)**: Manages user interaction, routing, and displays pages based on authentication status.

## Routes

### Public Routes

- `/login` - User login page.
- `/register` - User registration page.

### Protected Routes

- `/dashboard` - Accessible only to authenticated users.

### Home Route

- `/` - A public route that displays the home page.

## Usage

- Register a new user on the `/register` page.
- Log in with the registered credentials on the `/login` page.
- After login, you will be redirected to the `/dashboard` page.
- If logged in, attempting to access `/login` or `/register` will redirect you to the `/dashboard` page.
- The JWT token is stored in `localStorage` for session persistence.

## Technologies Used

- **Frontend**: React, React Router v6
- **Backend**: Node.js, Express.js, MongoDB, JWT
- **Libraries**: `axios`, `jwt-decode`, `dotenv`



