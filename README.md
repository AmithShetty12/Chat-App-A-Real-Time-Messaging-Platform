# Chat-App: A Real-Time Messaging Platform

## Table of Contents
- [Project Overview](#project-overview)
- [This Website Features](#this-website-features)
- [Setup and Instructions](#setup-and-instructions)
- [Project Structure](#project-structure)
- [Extensions](#extensions)
- [Further Implementations](#further-implementations)
- [Acknowledgments](#acknowledgments)

## Project Overview
As part of the Bright Network Technology Academy, we were assigned a group project to research, plan, and develop a Full-stack project—a chat app in 10 days.

## This Website Features
- Login functionality
- Registration
- Add/remove friends
- Chat with friends
- Switch chats

## Setup and Instructions

### 1. Ensure MongoDB is Running

#### i. Check MongoDB Service Status:
Open Command Prompt and run:
```sh
net start MongoDB
```

#### ii. Verify MongoDB is Running:
Open Command Prompt and run:
```sh
mongod
```

### 2. Update Dependencies
Ensure that all dependencies are up-to-date. Sometimes, older versions of Mongoose or MongoDB Node.js driver can cause issues:
```sh
npm update mongoose
```

### 3. Fix Vulnerabilities
While not directly related to the connection issue, it's a good practice to address any vulnerabilities:

Run npm audit:
```sh
npm audit
```

Fix vulnerabilities:
```sh
npm audit fix
```

Force fix if necessary (be cautious as this might introduce breaking changes):
```sh
npm audit fix --force
```

### 4. Steps to Ensure Both are Working:

#### i. Backend Setup:
Navigate to the `express.js_server` directory. Ensure your `index.js` (or the main server file) is correctly set up with the root route. Start the backend server:
```sh
npm install
npm start
```

#### ii. Frontend Setup:
Navigate to the `react.js_app` directory. Ensure your React application is correctly set up. Start the frontend server:
```sh
npm install
npm start
```

### Accessing the Application:
- Backend: Typically runs on [http://localhost:4000/](http://localhost:4000/) (depending on the port specified in your Express setup).
- Frontend: Typically runs on [http://localhost:3000/](http://localhost:3000/).

## Example Directory Structure:
```
├───express.js_server
│   ├───controllers
│   │     ├───ChatController.js
│   │     └───UserController.js
│   ├───models
│   │     ├───Chat.js
│   │     └───User.js
│   │
│   ├──routes
│   │      ├───Chat.js
│   │      └───User.js
│   │
│   ├───index.js
│   ├──package.json
│   └───package-lock.json
│
│
└───react.js_app
    ├───public
    │     ├───index.html
    │     ├───manifest.json
    │     └───robots.txt
    ├───src
    │    ├───components
    │    │      ├───Chat.css
    │    │      ├───Chat.js
    │    │      ├───FriendsList.css
    │    │      ├───FriendsList.js
    │    │      ├───Login.css
    │    │      ├───Login.js
    │    │      ├───Registration.css
    │    │      ├───Registratition.js
    │    │      ├───Search.css
    │    │      └───Search.js
    │    ├───containers
    │    │      ├───AppContainer.js
    │    │      ├───ChatContainer.css
    │    │      ├───ChatContainer.js
    │    │      └───UserContainer.js
    │    ├───App.css
    │    ├───App.js
    │    ├───App.test.js
    │    ├───index.css
    │    ├───index.js
    │    ├───reportWebVitals.js
    │    ├───setupTests.js
    │    └───UserContent.js
    ├──package.json
    └───package-lock.json
```

## Extensions
We have expanded on this full-stack project to include:
- Add multiple friends
- Multiple conversations
- Unfriend & Delete chats
- Encrypt stored password

## Further Implementations
Further functionalities we would like to develop into this website are:
- Group chats
- Pop-up window for notifications
- Delete accounts
- Typing bubble
- Account profile picture

## Collaborators
[Darshan J Baligeri](https://github.com/Darshan-Baligeri)
[Gagan K](https://github.com/Gagank30)
[Dhruva K](https://github.com/Dhruva6364)
