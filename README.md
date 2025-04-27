# Chat App

## Introduction
The **Chat App** is a real-time full-stack messaging application that allows users to chat instantly with each other. Built using **Socket.io** for live communication, it features user authentication, secure messaging, and a clean, responsive UI.  
Perfect for understanding how real-time apps work in production environments.

## Project Type
**Fullstack** (Frontend + Backend + Database)

## Deployed App
Frontend: [Link](https://chat-nu-gules.vercel.app)
Backend: [link](https://chat-ha97.onrender.com)

## Directory Structure
- frontend
```
src/
├── assets/
├── components/
│ ├── ChatWindow/
│ ├── ContactList/
│ ├── Login/
│ ├── Navbar/
│ ├── Signup/
├── pages/
│ ├── Home.jsx
│ ├── ChatRoom.jsx
├── context/
│ ├── AuthContext.jsx
├── utils/
│ ├── api.js
├── App.jsx
├── main.jsx
├── index.css
├── App.css
.env
.gitignore
package.json
vite.config.js
```

- backend
```
src/
├── config/
│ ├── db.js
├── controllers/
│ ├── authController.js
│ ├── chatController.js
├── middleware/
│ ├── authMiddleware.js
├── models/
│ ├── User.js
│ ├── Message.js
├── routes/
│ ├── authRoutes.js
│ ├── chatRoutes.js
├── utils/
│ ├── generateToken.js
server.js
.env
.gitignore
package.json

```

## Features
- **User Authentication:** Secure sign-up, login, and logout functionality using JWT tokens.
- **Real-time Messaging:** Instant one-to-one messaging using **Socket.io** for real-time communication.
- **User Status:** Show online/offline status of users in real-time. Offline users can be hidden via settings.
- **Profile Page:** Each user has a personalized profile page with the option to update details.
- **Image Sharing:** Send and receive images in chat.
- **Responsive UI:** A mobile-friendly and desktop-responsive interface.
- **Theme Selection:** Users can select between different themes (light/dark mode) for a customized experience.
- **Protected Routes:** Secure routes with authentication middleware using JWT.
- **MongoDB Integration:** Persistent user and chat storage, ensuring data is stored reliably.
- **Send Text & Media:** Users can send both text and media messages in chat.
- **Profile Customization:** Option for users to customize their profile.
- **Logout:** Logout functionality for secure session management.
- **React Context API:** Global state management for storing user info and chat data.
- **Mobile & Desktop Support:** Fully responsive interface for mobile and desktop users.


## Installation & Getting started
Detailed instructions on how to install, configure, and get the project running. For BE/FS projects, guide the reviewer how to check mongodb schema etc.

```bash
git clone https://github.com/PoojaSingh31github/Chat-App.git
npm install
npm run dev
```

## Screenshots

### Login Page
![image](https://github.com/user-attachments/assets/7b94f37c-3bdc-48d6-8770-42a6f835db1e)

### Login Page (Phone)
![image](https://github.com/user-attachments/assets/bbf5b10b-8f60-4529-a1e2-8bae465e7387)

### Message Page
![image](https://github.com/user-attachments/assets/25f11b11-ad1a-4b4a-9e0c-66261aa0df95)

### Message Page (Phone)
![image](https://github.com/user-attachments/assets/4db6e2a3-3fd6-41a6-9ab0-b19f8f912d0b)

### Setting Page
![image](https://github.com/user-attachments/assets/45e62f76-42c9-44d0-9c64-af592c6b7473)

### Setting Page (Phone)
![image](https://github.com/user-attachments/assets/bf399baa-c1c4-4a31-93d4-d72fa8e1c136)

### profile Page
![image](https://github.com/user-attachments/assets/5cc4756d-1b4e-4049-9111-b4b5292e5eed)

### profile Page (Phone)
![image](https://github.com/user-attachments/assets/35f81297-e21a-4426-a018-62b3d23af202)

## Credentials
### login credentials 
- **email** - test1@gmail.com
- **Password** - 123456

# Backend API Endpoints (Chat App)

## Authentication Routes
- **POST** `/api/auth/register`  
  ➔ Register a new user.

- **POST** `/api/auth/login`  
  ➔ Login with email and password.

- **GET** `/api/auth/profile`  
  ➔ Get authenticated user's profile (Protected Route).

---

## Chat Routes
- **POST** `/api/chat/send/:receiverId`  
  ➔ Send a message to another user.

- **GET** `/api/chat/messages/:receiverId`  
  ➔ Get all chat messages between the authenticated user and another user.

---

## Backend (.env)

- `MONGODB_URI` : MongoDB connection string.
- `PORT` : Port number for the backend server.
- `JWT_SECRET` : Secret key for JWT Authentication.
- `NODE_ENV` : Set environment (`development` or `production`).
- `CLOUDINARY_CLOUD_NAME` : Cloudinary Cloud name for storing images.
- `CLOUDINARY_API_KEY` : Cloudinary API Key.
- `CLOUDINARY_API_SECRET` : Cloudinary API Secret.
- `FRONTEND_URL` : URL of the frontend app.

## Frontend (.env)

- `VITE_MODE` : Set to `development` or `production`.


## Technology Stack

### Frontend:
- **Vite**
- **Context-API**
- **Xyflow library**
- **CSS / Tailwind CSS** (for styling)

### Backend:
- **Node.js**
- **Express.js**
- **MongoDB** (for data storage)
---

# Notes
- ⚡ Make sure you **replace sensitive information** if deploying publicly.
- 🛡️ Do **not commit** your `.env` file to GitHub or any public repo.
- 🚀 Make sure both frontend and backend `.env` files are properly configured before starting the server.

---
