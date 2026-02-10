# Login System Setup

## Prerequisites
- Node.js installed
- MongoDB installed and running
- npm or yarn package manager

## Installation Steps

### 1. Install Dependencies
```
npm install
```

### 2. Configure Environment Variables
The .env file is already created with default values:
- MongoDB URI: mongodb://localhost:27017/loginDB
- JWT Secret: your_jwt_secret_key_here
- Port: 5000

### 3. Start MongoDB
- Windows: `mongod`
- macOS/Linux: `brew services start mongodb-community`

### 4. Run the Server
- Development Mode: `node server.js`
The server will start on [http://localhost:5000](http://localhost:5000)

### 5. Access the Frontend
Open `login.html` in your browser or serve it with a local server.

## API Endpoints

### Register
- `POST /register` with username, password, confirmPassword

### Login
- `POST /login` with username and password

## Features
- User registration with password confirmation
- Secure login with JWT authentication
- Password hashing with bcryptjs
- MongoDB database
- Error handling and validation
- Responsive frontend
- Token-based authentication
