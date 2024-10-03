# Expense-Manager
This project consists of a React frontend (using Vite), a Node.js backend (using Express), and MongoDB as the database.

# Prerequisites
- Install Docker on your machine.
- Sign up for Clerk to get your publishable API key for authentication.

# Setup Clerk Authentication
- Sign up on Clerk and obtain your publishable key from the Clerk dashboard.
- Create a .env.local file in the client/ directory and add the following line: VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key

# Setup MongoDB Connection
- Create a .env file in the server/ directory and add your MongoDB URI: MONGODB_URI=mongodb+srv://<your-username>:<your-password>@cluster0.mongodb.net/<your-dbname>?retryWrites=true&w=majority
- Replace <your-username>, <your-password>, and <your-dbname> with your actual MongoDB credentials and database name.
- The server will automatically use this URI to connect to MongoDB.

# Running the Application with Docker Compose
Step 1: Clone the Repository:
- git clone https://github.com/farooqammar51/sit725-2024-t2-prac8.git
- cd sit725-2024-t2-prac8

Step 2: Build and Start the Containers
- Build and start all services (client, server, and MongoDB) using Docker Compose:
- docker-compose up --build

This will:
- Build the Docker images for the client and server.
- Set up and run the MongoDB service.
- Start the containers for the client, server, and database.

# Access the Application:
- Client (React App): Open your browser and go to http://localhost:4173.
- API (Server): The server API is running at http://localhost:3001.

Step 3: Stopping the Application
- When you're done, you can stop and remove the containers with: docker-compose down
