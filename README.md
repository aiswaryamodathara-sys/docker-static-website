Docker Static Website

Project Overview

This is a beginner-level DevOps project that demonstrates how to containerize a static website using Docker and Nginx.

The website is created using HTML and served through an Nginx web server running inside a Docker container.

Technologies Used

- Docker
- Nginx
- HTML

Project Structure

docker-static-website/
├── Dockerfile
├── index.html
└── README.md

How It Works

1. The website content is created using "index.html".
2. The Dockerfile uses the Nginx Alpine image as the base image.
3. The "COPY" instruction copies the HTML file into the Nginx web directory.
4. A Docker image is built from the Dockerfile.
5. A container is created and started from the image.
6. The website can be accessed through a web browser using port mapping.

Dockerfile Explanation

- "FROM nginx:alpine" — Uses the lightweight Nginx Alpine image as the base image.
- "COPY index.html /usr/share/nginx/html/index.html" — Copies the HTML file into the Nginx web directory.

How to Run the Project

1. Clone the repository

git clone https://github.com/aiswaryamodathara-sys/docker-static-website.git

2. Navigate to the project directory

cd docker-static-website

3. Build the Docker image

docker build -t my-website .

4. Run the Docker container

docker run -d --name my-website-container -p 8080:80 my-website

5. Access the website

Open your browser and visit:

"http://localhost:8080"

Learning Outcomes

- Understanding Docker images and containers.
- Writing a basic Dockerfile.
- Building a Docker image.
- Running a container.
- Understanding port mapping.
- Hosting a static website using Nginx inside Docker.

Conclusion

This project helped me understand the basics of Docker containerization and how to serve a static website using Nginx inside a Docker container. 
