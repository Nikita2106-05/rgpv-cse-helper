# RGPV CSE Helper – Notes, PYQs & Important Questions

A one-stop, single-page web application built with the MERN stack, designed to provide RGPV Computer Science students with easy access to essential study materials like notes, previous year questions (PYQs), and important questions in a structured and intuitive flow.

## 📸 Screenshots

*(It's highly recommended to add screenshots here to showcase your project. For example: a screenshot of the main page, the login popup, and the notes section after login.)*

![Home Page Screenshot](https://via.placeholder.com/800x400.png?text=Home+Page+Screenshot)
*Screenshot of the main user interface.*

## ✨ Core Features

-   **📚 Structured Material Flow:** Select a semester (1-8), then a subject to view relevant materials.
-   **📄 Direct PYQ Access:** Download Previous Year Question papers directly without needing to log in.
-   **🔐 Protected Content:** Access to curated Notes, Important Questions, and Must-Do PYQs requires user authentication.
-   **🔑 JWT Authentication:** Secure user registration and login system using JSON Web Tokens.
-   **⚡ Single-Page Application:** A seamless and fast user experience built with React, with no page reloads.
-   **📱 Responsive Design:** Fully responsive UI built with TailwindCSS, accessible on any device.
-   **📂 File Uploads:** An administrative feature for uploading PDF notes and managing materials.

## 💻 Tech Stack

-   **Frontend:** React.js, TailwindCSS
-   **Backend:** Node.js, Express.js
-   **Database:** MongoDB (with MongoDB Atlas)
-   **Authentication:** JSON Web Tokens (JWT)
-   **File Handling:** Multer for server-side file uploads
-   **State Management:** React Context API or Redux

## 📂 Project Structure

rgpv-cse-helper/
│
├── backend/
│ ├── config/
│ ├── controllers/
│ ├── models/
│ ├── routes/
│ ├── middleware/
│ ├── uploads/ # Stores uploaded PDF files
│ ├── .env # Environment variables
│ ├── server.js
│ └── package.json
│
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── context/
│ │ └── ...
│ ├── package.json
│ └── ...
│
├── .gitignore
├── README.md
└── package.json

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You must have the following software installed on your machine:
-   [Node.js](https://nodejs.org/en/) (v16 or newer recommended)
-   [npm](https://www.npmjs.com/) (usually comes with Node.js)
-   A MongoDB database. You can either:
    -   Install it locally ([MongoDB Community Server](https://www.mongodb.com/try/download/community))
    -   Use a free cloud cluster from [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register) (Recommended)

### Installation & Setup

**1. Clone the Repository**
```bash
git clone https://github.com/your-username/rgpv-cse-helper.git
cd rgpv-cse-helper

2. Backend Setup

# Navigate to the backend directory
cd backend

# Install dependencies
npm install

# Create a .env file in the backend/ directory
touch .env

Now, open the .env file and add the following environment variables.

File: backend/.env

# Port for the backend server
PORT=5000

# Your MongoDB Atlas connection string (or local connection string)
# Make sure to add your database name before the '?'
MONGO_URI=mongodb+srv://<username>:<password>@yourcluster.mongodb.net/rgpv-cse-helper?retryWrites=true&w=majority

# A secret key for signing JWTs (can be any long random string)
JWT_SECRET=your-very-strong-and-secret-key

3. Frontend Setup

# Navigate to the frontend directory from the root folder
cd frontend

# Install dependencies

npm install

Running the Application

You need to run both the backend and frontend servers simultaneously. Open two separate terminals for this.

In Terminal 1 (from backend/ directory):

# This will start the backend server (usually on http://localhost:5000)

npm run dev

# or 'nodemon server.js' if you have nodemon installed

In Terminal 2 (from frontend/ directory):

# This will start the React development server (usually on http://localhost:3000)

npm start

Your application should now be running, with the frontend at http://localhost:3000 communicating with the backend at http://localhost:5000.
