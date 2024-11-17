YouTube Clone Website
This project is a YouTube clone built to replicate the basic functionality of YouTube using modern web development technologies. The app allows users to upload, view, search, and comment on videos, simulating a YouTube-like experience.

Features
Video Upload: Upload videos and share them with other users.
Video Playback: Watch videos with a custom video player.
Search: Search for videos based on title or description.
User Authentication: Secure user authentication with login and registration.
Like/Dislike: Like or dislike videos.
Comments: Post comments on videos.
Responsive Design: Fully responsive and mobile-friendly interface.
User Profiles: Users can manage their profiles and uploaded content.
Demo
You can try the live demo of the application here:
Live Demo

Technologies Used
Frontend
React.js: A JavaScript library for building user interfaces.
React Router: For handling client-side routing.
Axios: For making HTTP requests to the backend.
Material-UI: A React UI framework for responsive design and ready-to-use components.
HTML5 Video Player: For video playback functionality.
Backend
Node.js: A JavaScript runtime for server-side development.
Express.js: Web framework for building the backend API.
MongoDB: NoSQL database for storing user data, videos, and comments.
JWT (JSON Web Tokens): For user authentication and session management.
Cloudinary (or AWS S3): For video file storage and streaming.
bcrypt.js: For password hashing and security.
Setup and Installation
Prerequisites
Node.js: Ensure you have Node.js installed (version 14 or later).
MongoDB: Ensure you have MongoDB installed or use a cloud-based service like MongoDB Atlas.
Cloudinary Account (optional for video storage): You can sign up for free at Cloudinary or use an alternative like AWS S3 for video hosting.
Local Development Setup
1. Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/youtube-clone.git
cd youtube-clone
2. Install Backend Dependencies
Navigate to the backend directory and install the required dependencies.

bash
Copy code
cd backend
npm install
3. Setup Environment Variables
Create a .env file in the backend directory and add the following environment variables:

makefile
Copy code
PORT=5000
MONGO_URI=mongodb://localhost:27017/youtube-clone
JWT_SECRET=your-jwt-secret-key
CLOUDINARY_URL=your-cloudinary-url
Replace your-jwt-secret-key with a secret key of your choice.
Replace your-cloudinary-url with your Cloudinary API credentials, if you're using Cloudinary for video storage.
4. Start the Backend Server
Run the following command to start the backend server:

bash
Copy code
npm run dev
5. Install Frontend Dependencies
Navigate to the frontend directory and install the required dependencies.

bash
Copy code
cd frontend
npm install
6. Start the Frontend Development Server
Start the React development server.

bash
Copy code
npm start
Your application should now be running at http://localhost:3000.

Application Structure
bash
Copy code
/youtube-clone
  /backend          # Backend server and API
    /controllers    # Handle requests and responses
    /models         # MongoDB models (User, Video, Comment)
    /routes         # API routes
    /middleware     # JWT authentication middleware
    .env            # Environment variables
    server.js       # Backend server entry point
  /frontend         # React.js frontend
    /src
      /components   # React components (Header, VideoPlayer, etc.)
      /pages        # Pages for different routes (Home, VideoPage, etc.)
      /services     # API requests (Axios instance)
    public/index.html
    package.json
    .env            # Environment variables for frontend (optional)
API Endpoints
