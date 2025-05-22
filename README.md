
![image](https://github.com/user-attachments/assets/88daf1a6-76f1-40f6-b13b-07749d72c523)
GIFs are attached at the end.

Technologies Used
React and TailwindCSS for the frontend
Firebase for authentication
Node/Express for creating API endpoints
MongoDB for storing chat room members and their messages
Socket.io for making the app real-time
Basic Features
Users can register/login via email and password.
Profile page where users can update their avatar and display name.
Generate random avatars using DiceBear API
Users can create a room to chat with others.
Users can see online status.
Search functionality.
Chatting is real-time.
Emoji picker is also integrated.
Dark mode can be enabled.
Getting Started
To run this project locally, follow these steps:

Clone the repository.
Install the dependencies:
Navigate to the frontend directory and run npm install.
Navigate to the server directory and run npm install.
Set up Firebase:
Go to the Firebase Console.
Create a new project or select an existing one.
Go to the project settings or service accounts section.
Click on "Generate new private key" or a similar option.
Save the downloaded JSON file as serviceAccountKey.json.
Place the downloaded serviceAccountKey.json file in the server/config directory.
Set up Environment Variables:
In the frontend directory, create a new file named .env based on the .env.example file.
Update the values of the environment variables in the .env file with your Firebase configuration details.
In the root directory, create a new file named .env based on the .env.example file.
Update the values of the environment variables in the .env file according to your preferences. For example, set the PORT variable to specify the desired port for the server and set MONGO_URI to your MongoDB connection URI.
Run the server:
Navigate to the server directory and run npm run start.
Run the client:
Navigate to the frontend directory and run npm start.
The application will be accessible at http://localhost:3000.
Please make sure to keep the serviceAccountKey.json file and sensitive information secure and not commit them to version control.
