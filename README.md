# Kanban Board with JWT Authentication

## Description  
A Kanban board application with JWT (JSON Web Tokens) authentication. Users can securely log in, manage tasks on the board, and are redirected to the login page if unauthenticated or upon session expiration.

## User Story  
**As a member of an agile team**,  
**I want a Kanban board with a secure login page**,  
**So that I can securely access and manage my work tasks**.

## Acceptance Criteria  

### Login Page  
- Displays form inputs for `username` and `password`.  
- Redirects to the Kanban board upon successful JWT authentication.  
- Shows an error message for invalid credentials.  
- Stores JWT securely in `localStorage` for authenticated requests.  

### Authentication Handling  
- Logging out removes the JWT and redirects to the login page.  
- Unauthenticated access to the board redirects to the login page.  
- Inactive sessions expire, invalidate the JWT, and redirect to login upon next action.  

## Mock-Up  
### Login Page  
- Form with `username` and `password` fields.  
- Error message display for failed login attempts.  

### Kanban Board Page  
- Tasks organized into columns: **To Do**, **In Progress**, **Completed**.  
- Accessible only after authentication.  

---

## Installation  

### 1. Download Starter Code  
Download and unzip the [starter code](your-repo-link-here).  
*(Ensure you create your own repository with the starter code.)*  

### 2. Set Up the Project  
Clone your repository:  
```bash
git clone <your-repository-url>
cd <project-directory>

## 3. Install Dependencies


npm install

## 4. Configure Environment Variables
Create a .env file in the root directory and add:

env

JWT_SECRET=your_secret_key
DATABASE_URL=your_db_url

## 5. Start the Development Server

npm start
Access the app at: http://localhost:3000.

Deployment (Render)
Create a new Web Service on Render.

Push your code to GitHub and connect the repository to Render.

Set environment variables in the Render dashboard.

Deploy! The app will be live at the provided Render URL.

## Features
✅ Secure Login: JWT-based authentication.
✅ Task Management: Kanban columns for task status tracking.
✅ Session Expiry: Auto-logout after inactivity.
✅ Error Handling: Clear feedback for failed logins.

## Technologies Used
Frontend: HTML, CSS, JavaScript, React (if applicable)

Backend: Node.js, Express.js

Authentication: JWT

Database: [Specify if applicable, e.g., MongoDB, PostgreSQL]

## Contributing
Contributions are welcome! Fork the repo, submit issues, or open pull requests.