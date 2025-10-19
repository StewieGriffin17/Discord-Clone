# Discord Clone (Web) 🚀

A full-featured **web-based Discord clone** — real-time chat, friend invitations, rooms, and WebRTC signaling — built with **React + Redux** (frontend) and **Node.js + Express + MongoDB + Socket.IO** (backend).  
This project demonstrates user authentication, real-time messaging, room/peer signaling for WebRTC, and basic friend-request flow.

---

## 🔥Features

- User registration & login (JWT-based)
- Real-time one-to-one and room chats using **Socket.IO**
- Friend invitation flow (invite / accept / reject)
- Conversations & message persistence (MongoDB)
- Rooms management (create/join/leave)
- WebRTC signaling for peer-to-peer media (audio/video) using `simple-peer` (signaling over Socket.IO)
- Redux-powered React frontend with Material-UI components
- Basic input validation and API routes using Joi (request validation)

---

## 🧭 Tech Stack

**Frontend**
- React
- Redux (+ redux-thunk)
- react-router
- axios
- socket.io-client
- simple-peer (WebRTC)
- Material-UI

**Backend**
- Node.js + Express
- Socket.IO
- MongoDB (Mongoose)
- JWT (jsonwebtoken)
- bcryptjs (password hashing)
- joi + express-joi-validation (validation)
- dotenv (environment variables)

---

## 📁 Project Structure (key files)
```bash
Dicord Clone/
├─ backend/
│ ├─ controllers/
│ ├─ middleware/
│ ├─ models/
│ ├─ routes/
│ ├─ socketHandlers/
│ ├─ server.js 
│ ├─ serverStore.js
│ ├─ socketServer.js
│ └─ .env
│
├─ frontend/
│ ├─ src/
│ │ ├─ authPages/
│ │ ├─ Dashboard/
│ │ ├─ realtimeCommunication/ 
│ │ ├─ shared/
│ │ ├─ store/
│ │ ├─ api.js 
│ │ ├─ App.css
│ │ ├─ App.js 
│ │ └─ index.js
│ └─ public/
└─ README.md
```
---

## 🛠 Prerequisites

- Node.js (14+ recommended)
- npm
- MongoDB (Atlas or local)
- Optional for development: `nodemon` (for backend hot reload)

---

## ⚙️ Setup & Run (Development)

> The project uses two separate apps — **backend** (API & socket server) and **frontend** (React). Start both.

### 1. Backend

1. Open a terminal and go to the backend folder:

```bash
cd "Dicord Clone/backend"
```

2. Install dependencies:
```bash
npm install
```

3. Create a .env file with those - 
```bash
API_PORT=5002
MONGO_URI=your_mongodb_connection_string
TOKEN_KEY=your_jwt_secret
```

4. Run the server:
```bash
node server.js
```

### 2. Frontend

1. Open another terminal and go to the frontend folder:

```bash
cd "Dicord Clone/frontend"
```

2. Install dependencies:
```bash
npm install
```

3. Start the dev server:
```bash
npm start
```
---

## 🖼️ Screenshots

### Login & Signup Page
<table>
 <tr>
   <td> <img src="/screenshots/1.PNG"/></td>
   <td> <img src="/screenshots/2.PNG"/></td>
 </tr> 
</table>

### Dashboard Page
<img src="/screenshots/3.PNG"/>

### Add Friend
<img src="/screenshots/4.PNG"/>

### Invitation Received 
<img src="/screenshots/5.PNG"/>

### Invitation Accepted
<img src="/screenshots/6.PNG"/>

### Personal Chatting 
<img src="/screenshots/7.PNG"/>

### Group Opend
<img src="/screenshots/8.PNG"/>

### Group Call (Audio/Video) 
<img src="/screenshots/9.PNG"/>

### Screenshare functionality 
<img src="/screenshots/10.PNG"/>

### Logout 
<img src="/screenshots/11.PNG"/>

--- 
## 📝Author

**Anowarul Asif**  
📧 [Reach Me Here](mailto:anowarul.asif@gmail.com)  
🌐 [Portfolio](https://anowarulasif.netlify.app/) | 🔗 [LinkedIn](https://www.linkedin.com/in/anowarul-asif/) | 🐙 [GitHub](https://github.com/StewieGriffin17)

---

## ⭐ Contribute

Contributions are welcome! Follow these steps:
1. Fork the repository  
2. Create a new branch: `git checkout -b feature-name`  
3. Commit your changes: `git commit -m "Add feature"`  
4. Push to your fork: `git push origin feature-name`  
5. Open a Pull Request  

---

## 🛡️ License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) — feel free to use and modify it.