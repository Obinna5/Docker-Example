10-2-24

Simple Docker example for a Node.js application.
Docker is an application that helps build, test, adn deploy applications. It works with containerization and virtualization through the use of images and containers. 

Dockerfile: File used to run the commands for building the container
Images: Snapshot of containers that run the application
Container: Environment that packages the application with dependencies (libraries, configurations)

The main difference from Docker and Jenkins is that docker is a containerization application that focuses on running applications in containers. It is mainly for scaling of applications and can integrate with Jenkins to run apps on containers. 

Jenkins focuses on CI/CD of building, testing, and deploying changes through automation. It focuses on automating the software lifecycle. 

# Initialize a node project
1. npm init -y

# Use Express (web framework)
2. npm install express

# Create a simple app


# Write a Dockerfile
# Dockerfiles define the environment for the application, the image, and commands for running inside the container. 

3. Create a file called Dockerfile in the same directory 

# Build and run the image within the same directory
4. docker build -t node-app-example . 

# Run the container, with the localhost being port:3003 and container port: 3000
docker run -p 3003:3000 node-app-exaple

# Access the web app through https://localhost:3003

# Stop a container
docker stop <id>

# List containers
docker ps

# List images
docker images


# Remove a container
docker rm <id>


# Remove an image
docker rmi <id>