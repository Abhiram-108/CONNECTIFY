
![image](https://github.com/user-attachments/assets/88daf1a6-76f1-40f6-b13b-07749d72c523)
💬 Real-Time Chat Application
A full-stack real-time chat app built with React, TailwindCSS, Firebase, Node.js, Express, MongoDB, and Socket.io. It supports user authentication, avatar customization, chat rooms, emoji support, dark mode, and real-time messaging.

🚀 Technologies Used
Frontend
React.js – JavaScript library for building UI

TailwindCSS – Utility-first CSS framework

Firebase – For user authentication (email/password)

DiceBear API – For generating random avatars

Emoji Mart – Emoji picker integration

Dark Mode – Toggleable light/dark themes

Backend
Node.js & Express.js – RESTful API creation

MongoDB – Database for users, rooms, and messages

Socket.io – Real-time, event-based communication

🔧 Features
✅ Email/password-based registration and login

👤 User profiles with editable avatar and display name

🎲 Random avatars via DiceBear API

💬 Create or join chat rooms

🟢 Display online status of users

🔍 Search feature

⚡ Real-time chat with Socket.io

😊 Emoji picker support

🌗 Dark mode toggle

🛠️ Getting Started
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/your-username/chat-app.git
cd chat-app
2. Install Dependencies
Frontend
bash
Copy
Edit
cd client
npm install
Backend
bash
Copy
Edit
cd ../server
npm install
3. Set Up Firebase Authentication
Visit Firebase Console

Create/select a project

Enable Email/Password sign-in under Authentication

Navigate to Project Settings > Service Accounts

Click Generate new private key and download the JSON file

Rename the file to serviceAccountKey.json and place it in:

pgsql
Copy
Edit
server/config/serviceAccountKey.json
4. Configure Environment Variables
Frontend
Copy .env.example to .env in client/

Fill in your Firebase config:

ini
Copy
Edit
REACT_APP_API_KEY=your_firebase_api_key
REACT_APP_AUTH_DOMAIN=your_project.firebaseapp.com
REACT_APP_PROJECT_ID=your_project_id
REACT_APP_STORAGE_BUCKET=your_project.appspot.com
REACT_APP_MESSAGING_SENDER_ID=your_sender_id
REACT_APP_APP_ID=your_app_id
Backend
Copy .env.example to .env in server/

Fill in your values:

ini
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
5. Run the Project
Start the backend server
bash
Copy
Edit
cd server
npm run start
Start the frontend
bash
Copy
Edit
cd ../client
npm start
The app will be available at: http://localhost:3000

🗂 Project Structure
client/ – React Frontend (CRA)
pgsql
Copy
Edit
client/
├── public/
├── src/
│   ├── components/
│   ├── pages/
│   ├── context/
│   ├── App.js
│   └── index.js
├── .env
├── tailwind.config.js
└── package.json
server/ – Node/Express Backend
pgsql
Copy
Edit
server/
├── config/
│   └── serviceAccountKey.json
├── controllers/
├── models/
├── routes/
├── socket/
├── .env
├── server.js
└── package.json
⚠️ Important Security Note
Ensure .env files and serviceAccountKey.json are included in .gitignore and are never committed to version control.
