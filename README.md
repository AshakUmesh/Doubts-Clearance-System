# Doubts Clearance System

A MERN-stack Q&A platform where students post academic doubts and faculty or senior students respond — built for the M.Tech Software Systems Lab (SSL) course at NIT Calicut, Monsoon 2025.

## About this fork

This is my working fork of a team MERN project. The base scaffolding is from the class template.

- Original class template: [anusudeep/mern-project-template-SSLlab-monsoon2025](https://github.com/anusudeep/mern-project-template-SSLlab-monsoon2025)
- Team-adapted parent fork: [pratikjadhav2000/Doubts-Clearance-System](https://github.com/pratikjadhav2000/Doubts-Clearance-System)

## What it does

Students in a course can post doubts (questions) to a shared board. Faculty and senior students can browse, respond, and mark answers as resolved. Each user has an authenticated account, so posts and responses are tied to identity.

## My contributions

I worked primarily on the backend and full-stack integration for our 4-person team:

**Backend (Node.js + Express + MongoDB):**
- Designed the MongoDB schema for users, doubts, and responses
- Built the JWT-based authentication middleware — token generation on login, token verification on protected routes, user context injection into request objects
- Implemented REST API routes for user registration, login, doubt creation, doubt listing, and response posting

**Full-stack integration:**
- Wired the React frontend to backend APIs during the final UI setup phase
- Handled auth state management and API calls on the client side
- Debugged cross-stack integration issues to get end-to-end flows working (login → post doubt → view responses → mark resolved)

**My commits:** [view filtered commit history](https://github.com/AshakUmesh/Doubts-Clearance-System/commits/main/?author=AshakUmesh)

## Team

Four-member M.Tech team. My role: backend + full-stack integration.

## Tech stack

- **Frontend:** React
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT (jsonwebtoken)

## Getting started

Requires Node.js 18+ and MongoDB (local instance or MongoDB Atlas connection string).

```bash
# Clone
git clone https://github.com/AshakUmesh/Doubts-Clearance-System.git
cd Doubts-Clearance-System

# Install root dependencies
npm install

# Install server dependencies
cd server
npm install

# Create .env inside /server with:
#   MONGODB_URI=your_mongo_connection_string
#   JWT_SECRET=your_jwt_secret
#   PORT=5000

# Start the backend (from /server)
npm start

# In a new terminal, install and start the frontend (from /client)
cd ../client
npm install
npm start
```

Backend runs on `http://localhost:5000`, frontend on `http://localhost:3000`.

## Course context

**Software Systems Lab (SSL)**, M.Tech CSE program, National Institute of Technology Calicut, Monsoon 2025.
