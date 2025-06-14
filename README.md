# Project_350_Tuition_Finder
This is our Github repo for Project 350.
<h1>Project Name:</h1> 
<h3>TuitionHub.</h3>
<h1>Team Members:</h1>
<h3>1.Irfanul Huda(2020331060)</h3>
<h3>2.Tanjima Rahman Farny(2020331074)</h3>
<h3>3.Zakaria Ahmed Jim(2020331050)</h3>
TuitionHub
TuitionHub is a web platform connecting guardians seeking tutors with qualified educators. Guardians can create tuition posts, while tutors can browse and apply for opportunities. The platform supports filtering, application management, and user dashboards, with all transactions displayed in Bangladeshi Taka (৳).
Table of Contents

Features
Technologies Used
Installation
Usage
API Endpoints


Features

Guardian Features:
Create and manage tuition posts with details like subjects, budget, and schedule.
View and manage tutor applications (accept/reject).
Dashboard to track active posts and application statuses.


Tutor Features:
Browse and filter tuition posts by subject, location, budget, and teaching mode.
Apply to posts with a cover letter and proposed rate.
Dashboard to monitor application statuses

Student Features:
Can use ChatBot to study and analyse weakness.

General Features:
User authentication (login, logout, role-based access).
Responsive UI with animated transitions.
Real-time data fetching and error handling.
Currency support for Bangladeshi Taka (৳).



Technologies Used

Frontend:
React (TypeScript)
React Router for navigation
Framer Motion for animations
Lucide React for icons
Tailwind CSS for styling


Backend (assumed, not provided):
Node.js with Express
MongoDB for data storage
JWT for authentication


Other:
Axios for API requests
Vite (assumed for development server)



Installation
Follow these steps to set up the project locally.
Prerequisites

Node.js (v18 or higher)
npm or Yarn
MongoDB (local or Atlas)
Backend API server running (see API Endpoints)

Steps

Clone the repository:
git clone <link>
cd tuitionhub


Install dependencies:
npm install


Set up environment variables:Create a .env file in the root directory and add:
VITE_API_URL=http://localhost:5000

Adjust VITE_API_URL to match your backend API URL.

Run the backend server:Ensure the backend server is running (refer to your backend documentation). The default API URL is http://localhost:5000.

Start the development server:
npm run dev

The app will be available at http://localhost:5173 (or the port specified by Vite).


Usage

Register or log in:
Create an account as a guardian, tutor, or student.
Log in to access role-specific features.


Guardians:
Navigate to the dashboard to create a new tuition post.
View applications under "My Tuition Posts" and accept/reject tutors.


Tutors:
Go to the "Tuition Posts" page to browse opportunities.
Apply to posts with a cover letter and proposed rate.
Track applications in the dashboard.


Admins (if implemented):
Access the platform overview to manage users and posts.



API Endpoints
The frontend interacts with the following API endpoints (assumed based on the code):

GET /api/tuition-posts: Fetch all tuition posts with filters.
GET /api/tuition-posts/my/posts: Fetch posts created by the guardian.
GET /api/tuition-posts/my/applications: Fetch applications submitted by the tutor.
POST /api/tuition-posts/:postId/apply: Submit an application to a post.
PUT /api/tuition-posts/:postId/applications/:applicationId: Update application status (accept/reject).



Guidelines

Follow the existing code style (Prettier, ESLint if configured).
Write clear, concise commit messages.
Test your changes locally before submitting.
Ensure no sensitive data is committed (e.g., .env files).

License
This project is licensed under the MIT License. See the LICENSE file for details.
