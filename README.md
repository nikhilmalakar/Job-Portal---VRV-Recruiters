# VRV Security - Role-Based Access Control (RBAC) System

This project is a fully functional Role-Based Access Control (RBAC) system designed for VRV Security to manage users, roles, and permissions within the company. The system allows administrators to efficiently manage users and their associated roles, permissions, and access controls. It is built using the MERN stack: MongoDB, Express, React, and Node.js.

## Features

- **User Management:**
  - View and manage users with options to add, edit, or delete users.
  - Assign roles to users and manage their active/inactive status.
  
- **Role Management:**
  - Create, define, and edit roles for users.
  - Manage role-specific permissions (e.g., Read, Write, Delete).
  
- **Dynamic Permissions:**
  - Assign and modify permissions for different roles.
  - Clearly display permissions for ease of understanding and modification.
  
- **Admin Dashboard:**
  - A user-friendly interface for administrators to manage roles, permissions, and users.
  - Ability to see all users, roles, and permissions in a simple and intuitive dashboard.

- **API Integration (Optional):**
  - Simulate CRUD operations (Create, Read, Update, Delete) for users and roles via mock API calls.
  - Simulated server responses to validate functionality.

## Screenshots

![Admin Dashboard Screenshot](https://github.com/nikhilmalakar/Job-Portal---VRV-Recruiters/blob/main/screenshots/01Home.png)
![User Management Screenshot](https://github.com/nikhilmalakar/Job-Portal---VRV-Recruiters/blob/main/screenshots/post-a-job.png)
![Role Management Screenshot](https://github.com/nikhilmalakar/Job-Portal---VRV-Recruiters/blob/main/screenshots/job-description.png)
![Role Management Screenshot](https://github.com/nikhilmalakar/Job-Portal---VRV-Recruiters/blob/main/screenshots/all-jobs-candidate.png)


## Installation

Clone the repository:
```
https://github.com/nikhilmalakar/Job-Portal---VRV-Recruiters
cd Job-Portal---VRV-Recruiters
```
Install server dependencies:
```
cd server
npm install
```

Install client dependencies:
```
cd client
npm install
```

Create a .env file in the server directory and add the following:
```
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Start the development server:
```
cd server
npm run dev
```

Start the client:
```
cd client
npm start
```

## Usage/Examples

- Navigate to `http://localhost:3000` in your web browser.
- Create a user account with specific roles (Admin, User, Moderator, etc.).
- Use the admin dashboard to manage users and roles.
- Assign permissions dynamically to different roles.
- Modify user access levels and track changes effectively.

## SRS Summary

### Problem Statement

The task is to design a Role-Based Access Control (RBAC) system for VRV Security, enabling administrators to manage users, roles, and permissions securely and efficiently. The system should allow for a clear structure of user roles, enabling the proper allocation of permissions based on these roles.


#### Users
- Candidate: A job seeker who applies for jobs.
- Coordinator: Manages job postings and recruitment workflows.
- Recruiters: Screens candidates' resumes.
- Employers: Creates job postings.

#### Job Posting Flow
- Employer creates a job post, including a job description and an R1 check form.
- Coordinator approves the job post, assigns recruiters, and adds an R2 check form.
- Coordinator posts the job, making it live for candidates to apply.

#### Application Flow
- Candidate creates an account, views job postings, and applies by uploading a resume and completing the R1 check form.
- Recruiter reviews applications, completes the R2 check form, and shortlists candidates for the final stage.
- Shortlisted applications appear in both employers' and coordinators' dashboards.

### Additional Requirements

- **Role-based access control** for users.
- **Dynamic permission management** for roles.
- **Security practices** including input validation and error handling to ensure robustness.

## Tech Stack

**Client:** React, Redux, TailwindCSS

**Server:** Node.js, Express, Mongoose

**Database:** MongoDB

## Authors

- [@nikhilmalakar](https://github.com/nikhilmalakar)
