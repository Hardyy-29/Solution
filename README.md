🗳️ Real-Time Poll Rooms

A full-stack real-time polling application where users can create polls, share a link, and vote live while results update instantly across all connected users.

This project demonstrates real-time communication, REST API design, frontend state management, and production-ready backend practices using modern web technologies.

🚀 Features

✅ Create polls with multiple options
✅ Unique poll share link generation
✅ Real-time voting updates using WebSockets
✅ Live percentage bars and vote counts
✅ One vote per user (client-side + server-side protection)
✅ Optimistic UI updates for instant feedback
✅ Responsive and modern UI
✅ MongoDB persistent storage
✅ Input validation and edge-case handling

🧱 Tech Stack
Frontend

React (Vite)

Axios

Socket.IO Client

Inline styling (Dark theme UI)

Backend

Node.js

Express.js

Socket.IO

MongoDB Atlas

Mongoose

Database

MongoDB (Cloud Hosted)

🏗️ System Architecture
Client (React)
     │
     │ REST API (HTTP)
     ▼
Express Server ───── MongoDB
     │
     │ WebSockets (Socket.IO)
     ▼
Real-time Vote Updates

Flow

User creates a poll

Backend stores poll in MongoDB

Poll link is generated

Users join poll room via Socket.IO

Vote is submitted via API

Server updates DB

Server emits vote_update

All clients update instantly
