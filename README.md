# Real-Time Chat Application

## Overview

This project is a full-stack web chat application focused on real-time message exchange between users. The application supports both one-on-one and group chats and is designed to work seamlessly across mobile and desktop platforms. In addition to text-based messaging, the app allows users to exchange images and files.

## Features

- **Real-time Messaging**: Instant message delivery powered by WebSockets for seamless communication.
- **One-on-One Chat**: Direct messaging between two users.
- **Group Chat**: Create and participate in group conversations with multiple users.
- **Media Sharing**: Supports sending and receiving images and file attachments in the chat.
- **Cross-Platform**: Works on both mobile and desktop devices.
- **User Authentication**: Secure login and user identification to protect chat privacy.
- **WebSockets Backend**: Real-time data transfer using WebSockets for smooth, live updates.

## Technologies Used

### Frontend:
- **React**: For building the dynamic user interface.
- **HTML/CSS**: For structuring and styling the web app.
- **Socket.IO Client**: For handling WebSocket connections on the client side.

### Backend:
- **Node.js**: JavaScript runtime for backend development.
- **Express.js**: Web framework for handling API requests and routing.
- **Socket.IO Server**: For real-time bidirectional event-based communication between clients and the server.
- **MongoDB**: NoSQL database for storing user data, messages, and chat history.
- **Mongoose**: ORM for interacting with MongoDB through Node.js.
- **JWT (JSON Web Tokens)**: For secure user authentication and authorization.
- **Cloud Storage (Optional)**: Integration for storing and retrieving files and images shared in chat.

### Tools & Libraries:
- **Axios**: For making API requests from the client.
- **Multer**: Middleware for handling file uploads in Node.js.
- **Bcrypt**: For hashing passwords and securing user data.
- **CORS**: To enable cross-origin requests between frontend and backend.
- **Dotenv**: For managing environment variables.

## Getting Started

### Prerequisites
- **Node.js**: Ensure you have Node.js installed. [Download Node.js](https://nodejs.org/)
- **MongoDB**: Setup MongoDB either locally or use a cloud-based service like [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).

### Installation

1. Clone the repository:
```bash
   git clone https://github.com/your-username/your-repo.git
```
2. Navigate to the project directory:
```bash
   cd your-repo
```
3. Install server-side dependencies:
```   
   cd backend
   npm install
```
4. Install client-side dependencies:
```
   cd ../frontend
   npm install
```
5. Create a `.env` file in the root of your backend project and set up the following variables:
 ```
   PORT=5000
   MONGO_URI=your-mongodb-connection-string
   JWT_SECRET=your-secret-key
```
6. Start the backend server:
```
   npm run server
```
7. Start the frontend development server:
```   
   npm start
```
8. Open the app in your browser:
 ```
   http://localhost:3000
``` 

### Development Reference
This project is based on the real-time web chat tutorial referenced here:
[YouTube - WebSockets with React and Node.js](https://www.youtube.com/watch?v=Fzv-rgwcFKk).
We will customize and build on the features presented in the video to create a unique, scalable solution for real-time chat.

### Future Enhancements
- **Push Notifications**: Integration of push notifications for unread messages.
- **Read Receipts**: Implement read/unread message statuses in chats.
- **Typing Indicators**: Show when users are typing a message.
- **Online Status**: Display online/offline status for users in chat.
- **Message Reactions**: Enable users to react to messages with emojis or reactions.
- **Profile Customization**: Allow users to upload profile pictures and set statuses.
- **Video/Audio Calls**: Add real-time video and audio calling features using WebRTC.
