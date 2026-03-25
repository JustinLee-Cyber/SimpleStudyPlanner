📚 Study Planner
📖 Project Description

Study Planner is a web application built with Node.js, Express, and SQLite that allows users to manage study tasks efficiently. Users can register, log in, create tasks, mark them as completed, and track their progress. The app also includes a profile system where users can update their username, email, and password.

✨ Features
🔐 User authentication (register, login, logout)
📊 Dashboard with task overview
📝 Add, edit (status), and delete tasks
✅ Mark tasks as completed
📜 Task history with completion date
👤 User profile management (edit username, email, password)
🗄 SQLite database for persistent storage
🔌 REST API using Express
🌐 Simple EJS frontend
🛠 Tech Stack
Node.js
Express.js
EJS (templating engine)
SQLite (database)
bcrypt (password hashing)
express-session (authentication sessions)
🚀 Setup Instructions
1. Clone the repository
git clone <repo-url>
cd study-planner
2. Install dependencies
npm install
or go to: https://nodejs.org/en/download and install latest
version used: node-v24.14.1-x64
3. Run the application
node app.js
4. Open in browser
http://localhost:3000
👤 Test Account

You can use the following pre-created test account:

Username: Test1
Password: Test1
🔌 API Endpoints
Authentication
POST /register – Create a new user
POST /login – Log in a user
POST /logout – Log out a user
Tasks
GET /tasks – Get all tasks
POST /tasks – Create a new task
PUT /tasks/:id/done – Mark task as completed
DELETE /tasks/:id – Delete a task
Profile
GET /profile – View profile page
POST /update-profile – Update username, email, or password
📁 Project Structure
study-planner/
├── app.js
├── database/
│   └── db.js
├── routes/
│   ├── authRoutes.js
│   └── taskRoutes.js
├── middleware/
│   └── auth.js
├── models/
├── views/
│   ├── dashboard.ejs
│   ├── login.ejs
│   ├── register.ejs
│   └── profile.ejs
└── package.json
⚠️ Notes
Ensure the SQLite database is properly initialized on first run.
If you encounter issues, delete the database.db file and restart the server to recreate tables.
Sessions must remain active for protected routes to work.