# hrms-lite

#Project overview
HRMS Lite is a full-stack web application for managing employee records and daily attendance. Built with React, Node.js, Express, and MongoDB, it demonstrates RESTful APIs, frontend–backend integration, validation, error handling, and cloud deployment on Vercel and Render.

#Tech stack
Frontend
React.js (Vite)
Tailwind CSS
Axios
Backend
Node.js
Express.js
Database
MongoDB (MongoDB Atlas)
Mongoose ODM
Deployment
Frontend: Vercel
Backend: Render

#Steps to Run the Project Locally

1.
Clone the Repository
git clone https://github.com/<your-username>/hrms-lite.git
cd hrms-lite

2.
Backend Setup
cd backend
npm install
Create a .env file inside the backend folder:
MONGO_URI=your_mongodb_atlas_connection_string
Start the backend server:
npm start
Backend will run on:
http://localhost:5000

3.
Frontend Setup
cd frontend
npm install
npm run dev
Frontend will run on:
http://localhost:5173

4.
Local API Configuration
Ensure frontend/src/services/api.js contains:
baseURL: "http://localhost:5000/api"

#Assumptions
The system is designed for a single admin user
No authentication or authorization is required
Employees do not log in themselves
Attendance is manually marked by the admin
Internet connectivity is available for database access (MongoDB Atlas)

#Limitations
No authentication or role-based access control
No payroll, leave management, or reporting features
No edit/update functionality for employee records
Attendance records do not prevent duplicate entries for the same date
Designed as a lightweight demonstration project, not a full enterprise HRM


