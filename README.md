# Day 4 - Docker Task

## 🚀 Topics Covered
- Docker container lifecycle
- Detached mode
- Viewing container logs
- Stopping and removing containers
- Rebuilding images after code changes

## 📁 Files Included
- `Dockerfile`: Docker configuration for the Node.js app.
- `index.js`: Basic Node.js server.
- `package.json` & `package-lock.json`: Project dependencies.
- `.dockerignore`: Files/folders excluded from Docker context.

## 🐳 Docker Commands Used
```bash
# Build the image
docker build -t node-app .

# Run the container in detached mode
docker run -d -p 3000:3000 --name node-container node-app

# View logs
docker logs node-container

# Stop and remove container
docker stop node-container
docker rm node-container

# Rebuild after code changes
docker build -t node-app .
