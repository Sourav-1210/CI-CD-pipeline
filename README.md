# 🚀 CI/CD Pipeline with Jenkins & Docker

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/Sourav-1210/CI-CD-pipeline)
[![Docker](https://img.shields.io/badge/docker-enabled-blue.svg)](https://www.docker.com/)
[![Jenkins](https://img.shields.io/badge/jenkins-pipeline-orange.svg)](https://www.jenkins.io/)
[![Node.js](https://img.shields.io/badge/node.js-v18+-green.svg)](https://nodejs.org/)

A robust, automated CI/CD pipeline demonstrating the integration of **Jenkins**, **Docker**, and **Node.js**. This project automates the entire process from code commit to deployment in a containerized environment.

---

## 🛠 Features

- **Automated Builds**: Triggered on every push to the repository.
- **Containerization**: uses Docker for consistent environments.
- **Jenkins Orchestration**: Comprehensive pipeline management.
- **Efficient Deployment**: Automatic removal of old containers and deployment of new ones.

---

## 🏗 Tech Stack

- **Backend**: Node.js & Express
- **CI/CD**: Jenkins
- **Containerization**: Docker
- **Version Control**: Git & GitHub

---

## 📂 Project Structure

```text
.
├── Screenshots/        # Pipeline execution screenshots
├── Jenkinsfile         # Jenkins declarative pipeline script
├── dockerfile          # Docker image configuration
├── index.js           # Main Express server app
├── package.json        # Project dependencies and scripts
├── .dockerignore       # Files excluded from Docker builds
└── .gitignore          # Files excluded from Version Control
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [Docker](https://www.docker.com/) installed and running
- [Jenkins](https://www.jenkins.io/) server configured

### 1. Local Setup

```bash
# Install dependencies
npm install

# Start the server
npm start
```

### 2. Docker Setup

```bash
# Build the image
docker build -t cicd-demo .

# Run the container
docker run -p 3000:3000 cicd-demo
```

### 3. Jenkins Configuration

1. Create a new **Pipeline** job in Jenkins.
2. Link your GitHub repository.
3. Jenkins will automatically pick up the `Jenkinsfile` and start the build.

---

## 📸 Screenshots

### Jenkins Pipeline Status
![Pipeline Status](./Screenshots/Screenshot%202026-04-23%20194856.png)

### Build History
![Build History](./Screenshots/Screenshot%202026-04-23%20195001.png)

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/Sourav-1210">Sourav</a>
</p>
