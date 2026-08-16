# Doubts Clearance System

A MERN-stack platform for [WHAT IT ACTUALLY DOES — see note below] built as part of the M.Tech SSL (Software Systems Lab) course at NIT Calicut, Monsoon 2025.

## About this fork

This is my working fork of the class MERN project. Original class template: [anusudeep/mern-project-template-SSLlab-monsoon2025](https://github.com/anusudeep/mern-project-template-SSLlab-monsoon2025). Team-adapted version: [pratikjadhav2000/Doubts-Clearance-System](https://github.com/pratikjadhav2000/Doubts-Clearance-System).

## My contributions

Worked primarily on the backend and full-stack integration for the team:

**Backend (Node.js + Express + MongoDB):**
- Designed the MongoDB schema for [doubts / users / responses — fill in what you actually modeled]
- Built out the Express middleware stack ([auth / validation / error handling — mention which ones]) 
- Implemented REST API routes for [core operations you built]

**Full-stack integration:**
- Wired the React frontend to the backend APIs during the final UI setup phase
- Handled state management and API integration on the client side
- Debugged cross-stack issues to get end-to-end flows working

**My commits:** [View filtered commit history](https://github.com/AshakUmesh/Doubts-Clearance-System/commits/main/?author=AshakUmesh)

## Team

Team project — 4 members. My role: backend + integration.

## Tech stack

- **Frontend:** React
- **Backend:** Node.js, Express
- **Database:** MongoDB
- **Other:** [any auth library, ORM, etc. you used]

## Getting started

Requires Node.js 18+ and MongoDB running locally (or a MongoDB Atlas connection string).

```bash
# Clone the repo
git clone https://github.com/AshakUmesh/Doubts-Clearance-System.git
cd Doubts-Clearance-System

# Install root dependencies
npm install

# Install server dependencies
cd server
npm install

# Install client dependencies  
cd ../client
npm install

# Create .env in server/ with:
# MONGODB_URI=your_mongo_connection_string
# JWT_SECRET=your_secret

# Start the backend (from /server)
npm start

# In a new
