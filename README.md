# Chat-App (MERN Stack)  
A real-time chat application built with the MERN stack (MongoDB, Express, React, Node.js) and Socket.IO.  
Allows users to register, login, chat one-to-one and in groups, manage profiles and more.

---

## 🔍 Features  
- User registration & authentication (JWT).  
- Real-time one-to-one and group chat via Socket.IO.  
- Create, rename, add / remove members from group chats.  
- Persistent chat history stored in MongoDB.  
- Profile updates (username, picture) for each user.  
- Responsive UI built in React.  
- Server API powered by Node.js + Express.  

---

## 🛠 Tech Stack  
- **MongoDB** — NoSQL database for users, chats and messages.  
- **Express.js** — Web framework for Node.js, handling routes & server logic.  
- **Node.js** — JavaScript runtime for server-side.  
- **React** — Front-end user interface.  
- **Socket.IO** — For bidirectional real-time communication between client & server.  

---

## 🚀 Getting Started  
### Prerequisites  
- Node.js installed (v14+ recommended).  
- MongoDB running (locally or via cloud).  
- Basic knowledge of environment variables (for secrets etc).  

### Installation & Setup  
1. Clone the repository:  
   ```bash
   git clone https://github.com/akshay3989/Chat-app-using-MERN-STACK.git
   cd Chat-app-using-MERN-STACK
2.Install server dependencies:

cd server
npm install

3.Install client dependencies:

cd ../client
npm install

4.Create a .env file (in server folder) and add something like:

MONGO_URI=<your-mongo-connection-string>
JWT_SECRET=<your-jwt-secret>
PORT=5000

5.Start the backend server:

cd ../server
npm run dev  # or npm start

6.Start the frontend client:

cd ../client
npm start

7.Open your browser and navigate to http://localhost:3000
 (or appropriate port) to use the app.

🎯 Usage

Register a new user or login with existing credentials.

From the chat interface, you can start a private chat with another user or create a group chat:

Choose a group name.

Add multiple users to the group.

Within a group you can send messages to all members in real-time.

You can also rename the group or remove members (if you’re the admin).

View chat history — previous messages are retrieved from the database.

Update your profile (name, picture) via profile settings.


PROJECT STRUCTURE  
/server
  ├── config/
  ├── controllers/
  ├── middlewares/
  ├── models/
  ├── routes/
  └── server.js
/client
  ├── src/
  │    ├── components/
  │    ├── pages/
  │    ├── context/
  │    ├── utils/
  │    └── App.jsx
  ├── public/
  └── package.json

🧪 Testing & Deployment

Ensure NODE_ENV=production when deploying.

Build the React client (npm run build) and serve it via your preferred web server (or via Express static files).

Ensure WebSocket (Socket.IO) communications are supported by your deployment environment (e.g., keep-alive, long-polling fallback, etc).

Secure credentials / secrets (Mongo URI, JWT secret) using environment variables and not committed files.
