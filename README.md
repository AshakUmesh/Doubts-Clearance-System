# Doubts Clearance System

A MERN-stack Q&A platform where NIT Calicut students post academic doubts, and faculty or senior students respond — with voting, reputation, comments, and an admin panel. Built for the M.Tech Software Systems Lab (SSL) course, Monsoon 2025.

**🔗 Live:** https://doubts-clearance-system.vercel.app

---

## About this fork

This is my working fork of a 4-person team MERN project. The base scaffolding is from the class template; the full-featured platform was built together by the team.

- Original class template: [anusudeep/mern-project-template-SSLlab-monsoon2025](https://github.com/anusudeep/mern-project-template-SSLlab-monsoon2025)
- Team-adapted parent fork: [pratikjadhav2000/Doubts-Clearance-System](https://github.com/pratikjadhav2000/Doubts-Clearance-System)

---

## What it does

A Stack Overflow-style Q&A platform for academic doubts:

- **Post doubts** with file/image attachments
- **Answer + comment** threads on each doubt
- **Upvote/downvote** doubts and answers
- **Reputation system** tracks user contributions
- **Admin panel** for moderation and user management
- **Google OAuth** login (with email/password as fallback)

---

## My contributions

I worked on the backend foundation and full-stack integration for our 4-person team:

**Backend (Node.js + Express + MongoDB):**
- Designed the MongoDB schema (users, doubts, answers, comments, votes, reputation)
- Built the JWT-based authentication middleware — token generation, verification on protected routes, request-level user context injection
- Set up the Express middleware stack (CORS, session, body parsing)

**Full-stack integration:**
- Wired the React frontend to backend APIs during the final integration phase
- Handled auth state on the client side (JWT storage, protected routes, redirects)
- Debugged cross-stack issues to get end-to-end flows working (login → post doubt → view/vote on responses)
- Contributed to team debugging across features during final integration

**Not my work (built by teammates):** the voting/reputation logic, admin panel, and Vercel deployment configuration.

**My commits:** [view filtered commit history](https://github.com/AshakUmesh/Doubts-Clearance-System/commits/main/?author=AshakUmesh)

---

## Team

Four-member M.Tech team:
- **Ashak Umesh** — backend schema, JWT middleware, integration *(this fork)*
- **Pratik Jadhav** — voting/reputation system, admin panel, deployment
- **Venkatesh Umesh**
- **Keval Umesh**

---

## Tech stack

**Frontend:** React (Vite)
**Backend:** Node.js, Express 5, ESM modules
**Database:** MongoDB (Mongoose ODM)
**Authentication:** JWT (jsonwebtoken) + Google OAuth 2.0 (Passport.js) + bcryptjs
**File uploads:** Multer
**Deployment:** Vercel (frontend + backend)

---

## Getting started

Requires **Node.js 18+**, **MongoDB** (local or Atlas), and **Google OAuth credentials** (Client ID + Secret from Google Cloud Console).

```bash
# Clone
git clone https://github.com/AshakUmesh/Doubts-Clearance-System.git
cd Doubts-Clearance-System

# Install server dependencies
cd server
npm install
```

Create `.env` in `/server` with:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
SESSION_SECRET=your_session_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
CLIENT_URL=http://localhost:5173
SERVER_URL=http://localhost:5000
PORT=5000
```

Then:

```bash
# Start backend (from /server)
npm run dev

# In a new terminal, install and start frontend (from /client)
cd ../client
npm install
npm run dev
```

- Backend: `http://localhost:5000`
- Frontend: `http://localhost:5173`

---

## Course context

**Software Systems Lab (SSL)**, M.Tech CSE program, National Institute of Technology Calicut, Monsoon 2025.
