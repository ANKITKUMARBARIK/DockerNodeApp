
# 🐳 Docker Project: MyApp

Welcome to the **Docker Project** for `MyApp`! This repository showcases how to containerize a Node.js application using Docker. Follow the instructions below to set up, build, run, and deploy the application using Docker.

## 📝 Table of Contents
- [📋 Overview](#overview)
- [🔧 Requirements](#requirements)
- [⚡ Quick Start](#quick-start)
- [🛠️ Setup Instructions](#setup-instructions)
- [🐳 Docker Commands](#docker-commands)
- [📦 Docker Hub](#docker-hub)
- [🔒 License](#license)
- [📞 Contact](#contact)

## 📋 Overview
This project demonstrates how to run a simple Node.js application inside a Docker container. The application serves a "Welcome to learn Docker.." message on port 8000.

## 🔧 Requirements
- Docker (latest version)
- Node.js (for local development)

## ⚡ Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/ANKITKUMARBARIK/DockerNodeApp.git
   ```

2. Navigate into the project directory:
   ```bash
   cd DockerNodeApp
   ```

3. Build the Docker container:
   ```bash
   docker build -t myapp .
   ```

4. Run the Docker container:
   ```bash
   docker run -d --name "webapp" --rm -p 8000:8000 myapp
   ```

5. Open your browser and visit `http://localhost:8000` to see the app running.

## 🛠️ Setup Instructions

### Building the Docker Image:
To build the Docker image manually, use the following command:
```bash
docker build -t myapp .
```

### Running the Container:
You can run the Docker container by mapping the appropriate ports:
```bash
docker run -d --name "webapp" --rm -p 8000:8000 myapp
```

### Stopping and Removing the Container:
To stop and remove the container:
```bash
docker stop webapp
```

## 🐳 Docker Commands

### List Images:
To list all Docker images:
```bash
docker image ls
```

### List Running Containers:
To list all running containers:
```bash
docker ps
```

### Pull an Image from Docker Hub:
To pull a pre-built image (like Nginx):
```bash
docker pull nginx
```

### Run Nginx in a Container:
Run Nginx in a Docker container:
```bash
docker run -d --name "engine" --rm -p 8000:80 nginx:latest
```

### Stop Nginx Container:
Stop the Nginx container:
```bash
docker stop engine
```

## 📦 Docker Hub

### Push Code to Docker Hub:
To share your app, push it to Docker Hub:
1. Create a repository on Docker Hub.
2. Build the image:
   ```bash
   docker build -t ankitkumarbarik/docker-webapp-demo:01 .
   ```
3. Push the image to Docker Hub:
   ```bash
   docker push ankitkumarbarik/docker-webapp-demo:01
   ```
4. Log out from Docker Hub:
   ```bash
   docker logout
   ```

### Example: Pull and Run App from Docker Hub
To pull and run the app from Docker Hub, use the following commands:
```bash
docker pull ankitkumarbarik/docker-webapp-demo:01
docker run -d --name "demoapp" --rm -p 8000:8000 ankitkumarbarik/docker-webapp-demo:01
docker stop demoapp
```

## 🔒 License
This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact
- **Email**: ankitbarik.dev@gmail.com
- **GitHub**: [ANKITKUMARBARIK](https://github.com/ANKITKUMARBARIK)

---

Happy Docking! 🎉
