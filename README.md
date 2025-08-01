Here’s a simple `README.md` file you can use for your **Dockerised Python Hello World** project. It explains the purpose, steps, and Docker commands you've used:

---

# Docker-Python-HelloWorld

This project demonstrates how to containerize a basic Python script using Docker.

## 🐍 What It Does

Runs a simple Python script (`helloworld.py`) inside a Docker container.

## 📁 Project Structure

```
project/
│
├── Dockerfile
├── helloworld.py
└── README.md
```

## 📦 Dockerfile

```Dockerfile
FROM python:latest
WORKDIR /usr/app/src
COPY helloworld.py ./
CMD [ "python", "./helloworld.py" ]
```

## 🧑‍💻 Setup Instructions

### 1. Create project directory and files

```bash
mkdir project
cd project
touch Dockerfile helloworld.py README.md
```

### 2. Write your Python script

**helloworld.py**

```python
print("Hello from Dockerised Python!")
```

### 3. Build and run with Docker

```bash
# Log in to DockerHub
sudo docker login

# Build Docker image
sudo docker build -t avinashtale99/pythonhelloworld .

# List Docker images
sudo docker images

# Run the container
sudo docker run avinashtale99/pythonhelloworld

# (Optional) Check running containers
sudo docker ps -a
```

### 4. Push to DockerHub

```bash
sudo docker push avinashtale99/pythonhelloworld
```

---

## 🐳 Notes

* Replace `avinashtale99` with your actual DockerHub username if different.
* Ensure Docker is installed and running on your system.
* You may need to install tools like `tree` using `sudo yum install tree` to visualize the file structure.

---


