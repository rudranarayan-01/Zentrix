# Social Media Application with MERN Stack and Socket.io

## Introduction
This is a full-stack social media application built using the **MERN stack** (MongoDB, Express.js, React.js, and Node.js) with **Socket.io** for real-time communication. The app allows users to create profiles, share posts, interact with others, and engage in real-time messaging.

## Features
- User Authentication (JWT-based Login & Signup)
- Profile Management
- Create, Read, Update, and Delete (CRUD) Posts
- Like and Comment on Posts
- Real-time Chat using Socket.io
- Friend Requests & Follow System
- Notifications System
- Responsive UI

## Technologies Used
- **Frontend**: React.js, Redux Toolkit, Tailwind CSS
- **Backend**: Node.js, Express.js, MongoDB (Mongoose ORM)
- **Real-time Communication**: Socket.io
- **Authentication**: JWT (JSON Web Tokens), bcrypt.js for password hashing
- **Database**: MongoDB with Mongoose

## Installation
### Prerequisites
Ensure you have the following installed:
- Node.js & npm
- MongoDB (local or cloud-based like MongoDB Atlas)

### Setup
#### 1. Clone the Repository:
```sh
git clone https://github.com/your-username/social-media-mern.git
cd social-media-mern
```

#### 2. Install Dependencies:
##### Backend:
```sh
cd backend
npm install
```
##### Frontend:
```sh
cd ../frontend
npm install
```

#### 3. Configure Environment Variables
Create a `.env` file in the `backend` folder and set the following values:
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

#### 4. Run the Application
##### Start Backend:
```sh
cd backend
npm start
```
##### Start Frontend:
```sh
cd frontend
npm start
```
The frontend should be accessible at `http://localhost:3000` and the backend at `http://localhost:5000`.

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|--------------|
| POST   | /api/auth/register | Register a new user |
| POST   | /api/auth/login | Login user |
| GET    | /api/users/:id | Get user profile |
| POST   | /api/posts | Create a post |
| GET    | /api/posts | Fetch all posts |
| PUT    | /api/posts/:id | Update a post |
| DELETE | /api/posts/:id | Delete a post |
| POST   | /api/messages | Send a message |
| GET    | /api/messages/:chatId | Fetch messages in a chat |

## WebSocket Events (Socket.io)
| Event | Description |
|--------|--------------|
| `connect` | Establish socket connection |
| `sendMessage` | Send a chat message |
| `receiveMessage` | Receive a new message |
| `userOnline` | Notify when a user comes online |
| `userOffline` | Notify when a user goes offline |

## Future Enhancements
- Video & Image Uploads
- Group Chats & Channels
- Story Feature (Similar to Instagram Stories)
- Dark Mode
- Admin Panel

## Contributing
Feel free to fork this repository and submit pull requests for improvements. Open issues for any bugs or feature requests.

## License
This project is licensed under the MIT License.



![chatApp 78d2335bf9c8e88a53b3](https://github.com/user-attachments/assets/ee4e6720-00e2-40c5-8317-3dce71cd0d5e)

