nfoCrucible

A simple news portal with a placeholder fake‑news detection feature powered by machine learning techniques (simulated results).

Table of Contents

About

Features

Tech Stack

Prerequisites

Installation

Backend

Frontend (Client)

Usage

Project Structure

Disclaimer

License

About

This application displays the latest news articles and provides a simulated fake‑news detection feature. While the UI is fully functional, the ML‑based detection is a placeholder and does not rely on a real trained model.

Features

Browse top headlines by category

User authentication with JWT (login/register)

Endpoint to simulate fake‑news prediction

Responsive React frontend

RESTful API with Node.js & Express

Data persistence using MongoDB

Tech Stack

Frontend: React, React Router, CSS

Backend: Node.js, Express, JWT, Nodemon

Database: MongoDB

Prerequisites

Node.js (v14+)

npm (v6+)

MongoDB (local or Atlas cluster)

Installation

Backend

Clone the repo and navigate into it:

git clone <your-repo-url>
cd InfoCrucible

Install dependencies:

npm install

Create a .env file in the root with the following variables:

MONGODB_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000

Start the backend server:

npm start

Frontend (Client)

Navigate to the client directory:

cd client

Install dependencies:

npm install

Start the React development server:

npm start

The frontend will launch at http://localhost:3000 by default and proxy API requests to the backend.

Usage

Open your browser to http://localhost:3000.

Browse news categories via the header navigation.

(Optional) Register or log in to simulate authenticated actions.

Use the Check Fake News button on any article details page to see a simulated verdict.

Project Structure

InfoCrucible/
├── client/            # React frontend (runs on port 3000)
│   ├── public/
│   └── src/
│       ├── components/
│       └── App.js
├── node_modules/
├── .env               # Environment variables for backend
├── package.json       # Backend dependencies & scripts
└── server.js          # Express app entry point

Disclaimer

Note: The fake‑news detection feature is currently a placeholder and does not use a real trained machine‑learning model. Results are simulated for demonstration purposes only.

License

This project is open source and available under the MIT License.

