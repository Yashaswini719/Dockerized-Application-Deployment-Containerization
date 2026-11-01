## Project Overview

This project focuses on automating the deployment of a FastAPI application using Docker, GitHub Actions, and AWS EC2. Instead of manually building and deploying the application whenever changes are made, the CI/CD pipeline automates the entire process.

Whenever new code is pushed to GitHub, GitHub Actions builds the Docker image, pushes it to Docker Hub, and deploys the updated application to an AWS EC2 instance.

The project provides hands-on experience with Docker containerization, cloud deployment, CI/CD automation, and managing applications in a Linux environment.

## Technologies Used

| Technology | Purpose |
|---|---|
| FastAPI | Building REST API endpoints |
| Docker | Packaging the application into containers |
| GitHub | Managing application source code |
| GitHub Actions | Automating the CI/CD pipeline |
| AWS EC2 | Hosting the application |
| Docker Hub | Storing and managing Docker images |
| Linux | Managing the server and deployment environment |

## Key Features

- **FastAPI Application:** Provides two REST API endpoints:
  - `GET /` – Returns a welcome message: "Hello from DevOps App".
  - `GET /health` – Checks whether the application is running.

- **Docker Containerization:** Packages the application and its dependencies into a portable Docker container.

- **Automated CI/CD Pipeline:** Uses GitHub Actions to trigger the deployment workflow whenever code changes are pushed to the repository.

- **Docker Hub Integration:** Builds and pushes updated Docker images to Docker Hub.

- **AWS EC2 Deployment:** Connects to the EC2 instance through SSH and deploys the latest Docker image.

- **Secure Configuration:** Uses GitHub Secrets to store deployment credentials and SSH authentication details securely, without exposing them in the source code.