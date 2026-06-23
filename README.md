# 🚀 Helm Static Website Project

A modern **static website deployment project** using **Docker, Kubernetes, and Helm**.  
This project demonstrates how to containerize a simple frontend and deploy it on Kubernetes using Helm charts.

---

## 📌 Project Overview

This project includes:

- A responsive static website (HTML + CSS)
- Dockerized Nginx server to serve the frontend
- Kubernetes deployment managed by Helm
- NodePort service for external access

---

## 🏗️ Architecture
Frontend (HTML/CSS)
↓
Docker Image (Nginx)
↓
Kubernetes Pod
↓
Helm Chart Deployment
↓
Service (NodePort / Port-Forward)

---

## 📁 Project Structure

```
helm-project/
│
├── index.html              # Static webpage
├── style.css               # Styling file
├── Dockerfile              # Docker configuration
│
├── helm-project/           # Helm chart directory
│   ├── Chart.yaml
│   ├── values.yaml
│   ├── charts/
│   ├── templates/
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   ├── _helpers.tpl
│   │   └── NOTES.txt
│
└── README.md
```

---

## ⚙️ Technologies Used

- HTML5
- CSS3
- Docker
- Kubernetes
- Helm
- Nginx

---

## 🐳 Docker Image

This project uses the following Docker image:

```
elsa888/helm-project:latest
```

---

## 🚀 How to Run This Project

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/helm-project.git
cd helm-project
```

---

### 2️⃣ Deploy using Helm

```bash
helm install helm-project ./helm-project
```

---

### 3️⃣ Check Deployment

```bash
kubectl get pods
kubectl get svc
```

---

### 4️⃣ Access Application

#### Option 1: NodePort

```
http://localhost:30080
```

#### Option 2: Port Forward (Recommended)

```bash
kubectl port-forward service/helm-project 8080:80
```

Then open:

```
http://localhost:8080
```

---

## 🔄 Upgrade Application

Modify `values.yaml` and run:

```bash
helm upgrade helm-project ./helm-project
```

---

## ⏪ Rollback Deployment

```bash
helm history helm-project
helm rollback helm-project 1
```

---

## 📦 Build & Push Docker Image (Optional)

```bash
docker build -t elsa888/helm-project:latest .
docker push elsa888/helm-project:latest
```

---

## 🎯 Learning Outcomes

By completing this project, you will understand:

- How Docker containerizes applications
- How Kubernetes runs and manages containers
- How Helm simplifies Kubernetes deployments
- How services expose applications externally
- Real-world DevOps workflow structure

---

## 🔥 Key DevOps Concepts Covered

- Containerization
- Kubernetes Pods & Services
- Helm Charts & Templating
- Release management (install, upgrade, rollback)
- NodePort vs Port-forward access

---

## 👨‍💻 Author

**Aqsa**  
DevOps / Full Stack Developer

---

## 📜 License

This project is open-source and available under the MIT License.
```

---

# 🚀 If you want next level upgrade

I can help you turn this into a **portfolio-grade DevOps project** with:

🔥 GitHub Actions CI/CD (auto build + deploy Helm)  
🔥 Ingress (custom domain like helm.local)  
🔥 Grafana + Prometheus monitoring  
🔥 Production-grade Helm structure  

Just tell me 👍
