Web Application Documentation
How to Run the Application Locally
Prerequisites:

Node.js installed on your machine.
Git installed on your machine (optional).
Clone the Repository:


git clone <repository_url>
Navigate to the Project Directory:


cd <project_directory>
Install Dependencies:


npm install
Start the Application:


npm start
Access the Application:
Open a web browser and navigate to http://localhost:8081.

Building the Docker Image and Running a Container
Build the Docker Image:


docker build -t yourusername/yourwebapp .
Replace yourusername with your Docker Hub username and yourwebapp with the name you want to give to your Docker image.

Run a Container Using the Image:


docker run -d -p 3000:3000 yourusername/yourwebapp
This command will run the container in detached mode (-d) and map port 3000 of the container to port 3000 of your local machine (-p 3000:3000).

Access the Application:
Open a web browser and navigate to http://localhost:3000.

Assumptions or Decisions Made During Development
Base Image: Chose the official Node.js image as the base image for simplicity and compatibility.
Dependency Management: Used npm for managing dependencies as it's commonly used in the Node.js ecosystem.
Exposing Port: Assumed the application runs on port 3000 by default, but this can be adjusted as needed.
Start Command: Assumed the start command specified in package.json is npm start, which is common for Node.js applications.
