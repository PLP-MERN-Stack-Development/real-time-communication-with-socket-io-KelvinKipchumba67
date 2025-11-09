# Real-Time Chat Application
A fullstack, real-time chat application built with Node.js, Express, Socket.io, and React. It features a global chat room, online user lists, and real-time typing indicators, all styled with Tailwind CSS.

## Features
Global Chat Room: All connected users can send and receive messages in real-time.

Real-Time Messaging: Uses WebSockets (Socket.io) for instant message delivery.

Online User List: Displays a list of all users currently in the chat.

System Messages: Notifies the room when a user joins or leaves.

Message History: Loads previous messages from the server when a user joins.

Responsive UI: Styled with CSS for a modern, clean interface on all devices.

Tech Stack
Backend
Node.js: JavaScript runtime environment.

Express: Web framework for the server and API.

Socket.io: Library for real-time, bidirectional event-based communication.

cors: Middleware for handling Cross-Origin Resource Sharing.

dotenv: For managing environment variables.

Frontend
React: A JavaScript library for building user interfaces.

Vite: Frontend build tool for a fast development experience.

socket.io-client: The client-side Socket.io library.

CSS

📁 Project Structure
For this project to run, it assumes you have two main folders, one for the server and one for the client.

chat-app-root/
├── server/
│ ├── node_modules/
│ ├── server.js
│ ├── package.json
│ └── .env
│
└── client/
├── src/
│ ├── components/
│ │ ├── Chat.jsx
│ │ ├── Chat.css
│ │ ├── JoinChat.jsx
│ │ ├── JoinChat.css
│ │ ├── MessageInput.jsx
│ │ ├── MessageInput.css
│ │ ├── MessageWindow.jsx
│ │ ├── MessageWindow.css
│ │ └── UserList.jsx
│ │ └── UserList.css
│ ├── App.jsx
│ ├── main.jsx
│ ├── socket.js
│ ├── SocketContext.jsx
│ └── index.css
├── node_modules/
├── package.json
└── .env.local
🏁 Getting Started
Prerequisites
Node.js (v18 or later recommended)

npm (or yarn)

Installation & Setup
Clone the repository:

Bash

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Set up the Backend (Server):

Navigate to the server directory:

Bash

cd server
Install dependencies:

Bash

npm install
Create an environment file named .env:

Bash

touch .env
Add the following variables to your .env file. (The client runs on port 5173 by default).

Code snippet

PORT=5000
CLIENT_URL=http://localhost:5173
Start the backend server:

Bash

node server.js
Your server should now be running on http://localhost:5000.

Set up the Frontend (Client):

Open a new terminal and navigate to the client directory:

Bash

cd client
Install dependencies:

Bash

npm install
Create a local environment file named .env.local:

Bash

touch .env.local
Add the following variable to your .env.local file to tell your React app where the server is:

Code snippet

VITE_SOCKET_URL=http://localhost:5000
Start the frontend development server:

Bash

npm run dev
Your React app should now be running on http://localhost:5173.

Open the App! Open http://localhost:5173 in your browser to use the chat application.
