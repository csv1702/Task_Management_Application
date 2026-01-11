# Task Management Application

A full-stack Task Management Application built with the MERN stack (MongoDB, Express, React, Node.js). This application enables users to register, authenticate securely using JWT tokens, and manage their tasks efficiently with a responsive and intuitive interface.

## Live Deployment Links

- **Frontend**: https://task-management-application-sigma-umber.vercel.app/login
- **Backend API**: https://task-management-application-axuk.onrender.com/

## Features

- **User Authentication**

  - User registration and login
  - JWT-based authentication with secure token management
  - Password validation and error handling

- **Authorization & Security**

  - Protected routes with role-based access control
  - JWT token verification on all API endpoints
  - Secure session management

- **Task Management**

  - Create, Read, Update, and Delete (CRUD) tasks
  - Mark tasks as completed or pending
  - Edit task details and descriptions
  - Delete completed or unwanted tasks

- **Search & Filtering**

  - Filter tasks by status (Pending / Completed)
  - Search tasks by title or description
  - Real-time filtering without page reload

- **User Interface**
  - Fully responsive design for desktop, tablet, and mobile
  - Clean and intuitive navigation
  - Form validation and user feedback
  - Loading states and error handling

## Tech Stack

### Frontend

- **React 18** with Vite for fast development and optimized builds
- **React Router** for client-side routing and protected routes
- **Axios** for HTTP communication with the backend
- **Tailwind CSS** for modern, utility-first styling
- **JavaScript (ES6+)** for application logic

### Backend

- **Node.js** runtime environment
- **Express.js** framework for building RESTful APIs
- **MongoDB** for data persistence
- **Mongoose** for MongoDB object modeling and validation
- **JWT (jsonwebtoken)** for authentication and authorization
- **bcryptjs** for secure password hashing

### Database

- **MongoDB Atlas** cloud-hosted MongoDB service

### Deployment

- **Frontend**: Vercel for automatic deployment and CDN
- **Backend**: Render for hosting the Node.js/Express server

## Project Structure

```
mern-auth-dashboard/
├── client/                    # React frontend application
│   ├── src/
│   │   ├── components/       # Reusable React components
│   │   ├── pages/            # Page components for routing
│   │   ├── context/          # React Context for state management
│   │   ├── services/         # API service layer (Axios)
│   │   └── App.jsx           # Main application component
│   ├── index.html            # HTML entry point
│   ├── package.json          # Frontend dependencies
│   ├── vite.config.js        # Vite configuration
│   └── tailwind.config.js    # Tailwind CSS configuration
│
├── server/                    # Express backend application
│   ├── models/               # Mongoose schemas (User, Task)
│   ├── routes/               # API route definitions
│   ├── controllers/          # Route handlers and business logic
│   ├── middleware/           # Custom middleware (auth, error handling)
│   ├── config/               # Configuration files (database, JWT)
│   ├── server.js             # Express server entry point
│   └── package.json          # Backend dependencies
│
└── README.md                 # Project documentation
```

## Setup Instructions

### Prerequisites

Ensure you have the following installed on your machine:

- **Node.js** (v16 or higher)
- **npm** (v8 or higher)
- **MongoDB Atlas account** (for cloud database)
- **Git** (for version control)

### Backend Setup

1. **Navigate to the server directory**

   ```bash
   cd mern-auth-dashboard/server
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Create a `.env` file in the server directory** with the following variables:

   ```
   PORT=5000
   MONGODB_URI=your_mongodb_atlas_connection_string
   JWT_SECRET=your_secret_key_for_jwt
   NODE_ENV=development
   ```

4. **Start the backend server**
   ```bash
   npm start
   ```
   The server will run on `http://localhost:5000`

### Frontend Setup

1. **Navigate to the client directory**

   ```bash
   cd mern-auth-dashboard/client
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Create a `.env.local` file** with the backend API URL:

   ```
   VITE_API_URL=http://localhost:5000/api
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```
   The frontend will run on `http://localhost:5173`

## Author

#### Chandra Shekhar Verma

#### https://github.com/csv1702
