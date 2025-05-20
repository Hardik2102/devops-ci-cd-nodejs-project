# DevOps CI/CD Project – Node.js App with Docker & Jenkins

## 🚀 Project Description
This is a simple Node.js application containerized using Docker and deployed via Jenkins CI/CD pipeline on AWS EC2.

## 🛠️ Tools Used
- Node.js + Express
- GitHub
- Docker
- Jenkins
- AWS EC2 (Free Tier)

## 📦 Docker Commands
```bash
docker build -t hardik-node-app .
docker run -d --name hardik-node-app -p 80:3000 hardik-node-app
```

## 📈 Jenkins Pipeline Stages
- Clone GitHub Repo
- Build Docker Image
- Deploy Docker Container

## 📸 Output
Visit `http://<your-ec2-public-ip>` to see the running app.

---

✅ Created with ❤️ by Hardik Parmar
