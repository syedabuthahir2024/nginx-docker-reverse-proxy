# 🐳 NGINX Reverse Proxy + Docker Compose - DevOps Assignment

This project sets up a reverse proxy system using **Nginx**, **Docker Compose**, a **Golang** service, and a **Python** service.

---

## 📁 Project Structure

.
├── docker-compose.yml
├── nginx
│ ├── nginx.conf
│ └── Dockerfile
├── service_1/ # Golang App
│ ├── Dockerfile
│ └── (source code)
├── service_2/ # Python App
│ ├── Dockerfile
│ └── (source code)
└── README.md


---

## 🚀 How to Run

### 1️⃣ Prerequisites:
- Docker
- Docker Compose

### 2️⃣ Start the system:
```bash
docker-compose up --build

Once started, access services at:

http://localhost:8080/service1

http://localhost:8080/service2

🌐 NGINX Routing
Nginx is configured as a reverse proxy that listens on port 8080.

It:

Routes requests with /service1 to the Golang backend

Routes requests with /service2 to the Python backend

Logs all incoming requests with timestamp and URL path

❤️ Bonus Features
✅ Health checks added for both services via docker-compose.yml

✅ Clean and modular Docker setup

✅ Nginx logs all requests with time and path using access_log

🧠 Author
Mr. Syed Abuthahir
DevOps Intern Assignment
