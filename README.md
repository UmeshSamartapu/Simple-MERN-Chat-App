# 💬 Real-Time Chat Application

A simple yet modern full-stack real-time chat app that enables users to join chat rooms and exchange messages instantly. Built using **Socket.IO**, **Express.js**, **MongoDB**, and **Vanilla JavaScript** with a clean TailwindCSS-based UI.

---

## 🧠 Project Summary

- 🎯 **Goal**: Build a real-time chat platform supporting rooms, message broadcasting, and chat history.
- 🧰 **Tech Stack**:
  - **Frontend**: HTML, TailwindCSS, Vanilla JavaScript
  - **Backend**: Node.js, Express.js
  - **Realtime Engine**: Socket.IO
  - **Database**: MongoDB (for message persistence)
- 📦 **Deliverable**: A fully working chat system where multiple users can join rooms and communicate in real-time.

---

## 🗂️ Folder Structure

```bash
chat-app/│
├── server/
├── public/
│ ├── index.html # Frontend UI
│ └── script.js # Client-side Socket.IO logic
│ ├── server.js # Express + Socket.IO backend
│ ├── .env # Environment variables (MongoDB URI)
│ └── package.json # Backend dependencies
│
├── .gitignore
└── README.md # Project documentation
```

---

## 🚀 Live Demo

> To test locally, follow the setup instructions below and open `http://localhost:3000`

---

## ⚙️ Features

- ✅ Join any chat room by entering a username and room name.
- 💬 Send/receive messages instantly using WebSockets.
- 🧑‍🤝‍🧑 See notifications when users join or leave.
- 🕓 Chat history is fetched from MongoDB for new users.
- 🌐 Responsive and elegant UI using TailwindCSS.

---

## 🛠️ Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) installed
- A [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) cluster or local MongoDB

### 1. Clone the repo

```bash
git clone https://github.com/your-username/chat-app.git
cd chat-app/server
```
2. Install dependencies
```bash
npm install
```

3. Create .env file
Inside the server/ directory, create a file named .env:
```bash
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/?retryWrites=true&w=majority
Replace <username> and <password> with your actual MongoDB credentials.
```

4. Run the server
```bash
node server.js
Server will run on http://localhost:3000
```

### 🖥️ Frontend Overview

The public/index.html page includes:

Join Room Form

Real-time chat box with messages

TailwindCSS styling

script.js that handles Socket.IO events for sending/receiving messages

### 🔌 Socket.IO Events

#### Client → Server:
- **join room:** Join a specific room

- **chat message:** Send a message

#### Server → Client:
- **chat message:** Broadcast a message to all users in the room

- **user notification:** Notify users when someone joins/leaves

- **chat history:** Load past messages when joining

### 🧩 Future Enhancements (Optional)

- 🔐 JWT-based authentication

- 📱 React-based frontend

- 📋 User typing indicators

📦 Dockerize the app

🧪 Add tests (Mocha/Chai)

### 🤝 Contributing
Feel free to fork the project, open issues, or submit PRs to improve it!

### 📝 License
This project is open source and available under the MIT License.

### 👨‍💻 Author
Built by Umesh Samartapu


