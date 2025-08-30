# ChronoStream.github.io
Chrono-Stream
Chrono-Stream is a sci-fi themed, real-time, anonymous chat application. It's built on the concept of "Temporal Resonance," where messages, or "echoes," are imprinted onto a global, shared timeline for all connected operators to see instantly.

This application provides a cinematic, hacker-style terminal interface to monitor the global echo network. Every echo broadcasted by any user appears on your screen in real-time, creating a feel of being connected to a stream of consciousness from the Matrix.

Features
Real-Time Global Stream: See messages from every user, anywhere in the world, as they are sent.

Anonymous Broadcasting: Users are identified only by a temporary, anonymous UserID.

Cinematic UI: A hacker-terminal aesthetic with a live status bar, glitch effects, and a scrolling feed of incoming "echoes."

Cross-Platform: As a web application, it runs on any device with a modern browser.

Serverless Backend: Powered by Firebase Firestore for a robust, scalable, and real-time database.

How It Works
Frontend: A single, self-contained index.html file using vanilla JavaScript and Tailwind CSS for styling. No complex frameworks are needed.

Backend: Google's Firebase Firestore is used as a serverless, real-time database. When a user broadcasts an echo, it's written to a public Firestore collection.

Real-Time Sync: The application uses a live onSnapshot listener from the Firestore SDK. This means that whenever a new document (an "echo") is added to the collection, the database pushes the update to all connected clients instantly.

Getting Started
To run this project, you will need to set up a free Firebase project.

Clone the repository:

git clone [https://github.com/your-username/chrono-stream.git](https://github.com/your-username/chrono-stream.git)
cd chrono-stream

Set up Firebase:

Go to the Firebase Console and create a new project.

Create a new Firestore database in your project.

In your Project Settings, add a new Web App.

Firebase will provide you with a firebaseConfig object.

Configure the Application:

The index.html file looks for global JavaScript variables (__app_id, __firebase_config, __initial_auth_token). For local development, you can replace these with your actual Firebase config details.

Open index.html:

You can open the index.html file in your web browser to start using the application. For the best experience, host it on a simple local server.

This project was created as a sci-fi concept app and is intended for creative and educational purposes.
