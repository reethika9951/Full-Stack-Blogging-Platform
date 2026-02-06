# Full-Stack-Blogging-Platform

Full Stack Blogging Platform – Project Documentation
1. Project Overview
Project Title
Full Stack Blogging Platform
Project Description
This project is a complete full stack blogging platform built using modern web technologies. It allows users to register, log in securely, create and manage blog posts, interact through comments, and manage their profiles. The application demonstrates real-world full stack development practices including authentication, protected routes, state management, API communication, and deployment.
Project Objectives
•	Build a production-ready full stack web application
•	Implement secure user authentication and authorization
•	Demonstrate React–Node–Database integration
•	Follow clean architecture and scalable code structure
•	Prepare a portfolio-level project suitable for MS applications and international job roles
________________________________________
2. Full Stack Architecture
Architecture Overview
The project follows a client–server architecture:
•	Frontend: React (TypeScript)
•	Backend: Node.js with Express
•	Database: MongoDB / Supabase (PostgreSQL)
•	Authentication: JWT (JSON Web Tokens)
•	API Communication: RESTful APIs over HTTP
Architecture Flow
1.	User interacts with React frontend
2.	Frontend sends HTTP requests to backend APIs
3.	Backend processes requests and communicates with database
4.	Backend returns JSON responses
5.	Frontend updates UI based on response
________________________________________
3. Authentication Flow
Authentication Type
•	JWT-based authentication
•	Access tokens stored securely
Authentication Steps
1.	User Registration
o	User submits name, email, password
o	Password is hashed before storing in database
o	JWT token is generated and returned
2.	User Login
o	Credentials validated on backend
o	JWT token issued on successful login
3.	Token Storage
o	Token stored in browser storage
o	Automatically attached to API requests
4.	Protected Routes
o	Frontend checks authentication state
o	Backend middleware verifies JWT
5.	Authorization
o	Only authenticated users can create, edit, or delete posts
________________________________________
4. Frontend–Backend Communication
Communication Method
•	RESTful APIs
•	Axios used on frontend
•	JSON request/response format
Example API Flow
•	Frontend sends request: POST /api/posts
•	Backend validates JWT
•	Backend processes request and stores data
•	Backend sends response
•	Frontend updates UI
Error Handling
•	Centralized error responses from backend
•	Frontend displays user-friendly messages
________________________________________
5. State Management
State Management Strategy
•	React Context API
•	Custom hooks for reusable logic
Managed State Includes
•	Authentication state
•	User information
•	Blog posts data
•	Loading and error states
Benefits
•	Global state access
•	Reduced prop drilling
•	Clean and maintainable code
________________________________________
6. Code Structure
Frontend Structure
frontend/
 ├── src/
 │   ├── components/
 │   ├── pages/
 │   ├── contexts/
 │   ├── hooks/
 │   ├── services/
 │   ├── lib/
 │   └── App.tsx
Backend Structure
backend/
 ├── src/
 │   ├── models/
 │   ├── routes/
 │   ├── middleware/
 │   ├── controllers/
 │   └── server.js
________________________________________
7. Technical Details
Algorithms & Logic
•	Password hashing using secure algorithms
•	JWT signing and verification
•	CRUD operations with database indexing
Data Structures
•	Users collection/table
•	Posts with relational references
•	Nested comment structure
Security Measures
•	JWT verification middleware
•	CORS configuration
•	Input validation
________________________________________
8. Setup Instructions
Prerequisites
•	Node.js
•	npm or yarn
•	MongoDB / Supabase account
Backend Setup
cd backend
npm install
npm run dev
Frontend Setup
cd frontend
npm install
npm run dev
Environment Variables
•	Database URL
•	JWT secret
•	API base URL
________________________________________
9. Testing Evidence
Manual Test Cases
Test Case	Description	Expected Result
Register User	Create new account	Account created successfully
Login User	Valid credentials	JWT token issued
Create Post	Authenticated user	Post created
Protected Route	Unauthenticated access	Redirect to login
Validation
•	Input validation on frontend
•	Server-side validation on backend
________________________________________
10. Visual Documentation
Screenshots Included
•	Login page
•	Registration page
•	Home feed with posts
•	Create/Edit post screen
•	Protected route behavior
________________________________________

12. Conclusion
This project demonstrates end-to-end full stack development using industry best practices. It is scalable, secure, and suitable for academic evaluation, portfolio presentation, and real-world use cases.
