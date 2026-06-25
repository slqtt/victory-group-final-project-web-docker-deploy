# Victory Group Final Project Web Docker Deploy
## 📸 Screenshots

### Personal Site

![Personal Site]<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/cb391139-0900-4c6b-9f2e-610454d4c22d" />


### TodoMVC

![TodoMVC]<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/6d138c1f-df28-4398-a084-2d364cfc9c22" />


## 📖 Project Overview

This project is a comprehensive Docker Compose deployment assignment developed by a three-person team. It contains two independent static front-end web applications, complete container orchestration configuration, and an automated CI/CD workflow based on GitHub Actions.

All web pages are fully displayed in English and include complete CSS styling and interactive JavaScript functionality.

---

## 🌐 Two Web Applications

### 1. Personal Site

Team member introduction homepage featuring:

- Three student profile photos
- Floating card animation
- Image zoom effect
- Click-to-popup detail functionality
- Independent Dockerfile for Nginx deployment

### 2. TodoMVC

An open-source static TodoMVC front-end project packaged and deployed using the lightweight `nginx:alpine` image.

---

## 📂 Directory Structure

```text
victory-group-final-project-web-docker-deploy/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── personal-site/
│   ├── index.html
│   ├── user1.jpg
│   ├── user2.jpg
│   ├── user3.jpg
│   └── Dockerfile
├── todomvc-master/
│   └── Dockerfile
├── docker-compose.yml
├── .gitignore
└── README.md
```

---

## 🚀 Local Deployment Guide

### 1. Clone the Repository

```bash
git clone https://github.com/slqtt/victory-group-final-project-web-docker-deploy.git
cd victory-group-final-project-web-docker-deploy
```

### 2. Build Images and Start Containers

```bash
docker compose up -d --build
```

### 3. Access the Applications

| Application | URL |
|------------|-----|
| Team Member Introduction Page | http://127.0.0.1:8080 |
| TodoMVC Task Management Page | http://127.0.0.1:8081 |

---

## ☁️ Cloud Server Deployment Guide

### 1. Install Docker and Docker Compose

Install Docker and Docker Compose on your Ubuntu cloud server.

### 2. Clone the Repository

```bash
git clone https://github.com/slqtt/victory-group-final-project-web-docker-deploy.git
cd victory-group-final-project-web-docker-deploy
```

### 3. Deploy the Project

```bash
docker compose up -d --build
```

### 4. Configure Firewall

Open ports **8080** and **8081** in your cloud server security group or firewall settings.

### 5. Access the Project

| Application | URL |
|------------|-----|
| Team Page | http://3.95.175.97:8080 |
| TodoMVC Page | http://3.95.175.97:8081 |

---

## 👥 Team Member Work Division

| Team Member | Responsibility | Contribution |
|------------|---------------|-------------|
| **Duan Junjie (20242179)** | Developed personal introduction website, wrote Nginx Dockerfile, configured GitHub Actions CI/CD pipeline | 33% |
| **Zhang Sheng (20242176)** | Integrated TodoMVC project, wrote `docker-compose.yml`, completed cloud deployment and debugging | 33% |
| **Li Mingze (20242177)** | Wrote project documentation, edited README, recorded demonstration video, maintained repository | 33% |

---

## 📌 File Specification Description

- The `.gitignore` file excludes:
  - `node_modules/`
  - `.pem` private key files
  - `.key` private key files

- Both front-end applications use the lightweight `nginx:alpine` image to reduce image size and save server resources.

- `docker-compose.yml` configures independent port mappings for the two services to avoid port conflicts during runtime.

---

## ⚙️ Technology Stack

- HTML5
- CSS3
- JavaScript
- Docker
- Docker Compose
- Nginx
- GitHub Actions
- CI/CD
- l145632：负责个人网站开发，参与项目协作
- zhishiluguo(Zhang Sheng 20242176): Responsible for TodoMVC project integration and docker-compose configuration, responsible for cloud server deployment debugging, and participating in the whole project collaboration.
