
# ☕️ Flask Docker App on EC2 with GitHub Actions

A Dockerized Flask application deployed on an EC2 instance with CI/CD using GitHub Actions.  
This project simulates a real-world DevOps scenario with automation, testing, and deployment pipelines.

This project was developed as part of my DevOps learning journey and includes automated tests, deployment pipelines, and dependency management.

---

## 🗂️ Table of Contents
- 🔍 Project Overview  
- 📐 Tech Stack  
- 📁 Project Structure  
- 🚀 How to Deploy  
- 🔐 Security Considerations  
- 🧠 What I Learned  
- 🛠️ Future Improvements  
- 📬 Contact  
- ✅ DevOps Learning Tracker  

---

## 🔍 Project Overview

This project includes:

- A Python Flask application  
- Dockerized deployment  
- CI/CD pipeline using GitHub Actions  
- Deployment on a self-hosted EC2 instance  
- Renovate integration for automatic dependency updates

---

## 📐 Tech Stack

| Layer              | Technology                        |
|--------------------|------------------------------------|
| App & API          | Flask (Python)                    |
| Containerization   | Docker, Docker Compose            |
| CI/CD              | GitHub Actions                    |
| Hosting            | AWS EC2 (self-hosted runner)      |
| Dependency Update  | Renovate                          |

---

## 📁 Project Structure
```bash
NouveauDepot/
├── app.py                 # Main Flask application
├── test.py                # Unit tests
├── Dockerfile             # Docker image definition
├── docker-compose.yml     # Docker multi-service setup
├── requirements.txt       # Python dependencies
├── templates/             # HTML templates
├── .github/workflows/     # GitHub Actions workflows
│   ├── CICD.yml
│   ├── CI.yml
│   └── Renovate.yml
├── renovate.json          # Renovate configuration
├── .gitignore             # Git & secrets exclusions
└── README.md              # This file
```



---

## 🚀 How to Deploy

### 1. Clone the repository
```bash
git clone https://github.com/redskot/NouveauDepot.git
cd NouveauDepot
```


### 2. Build and run with Docker Compose
`docker-compose up -d` 

Application available at: [http://localhost:5000](http://localhost:5000)

----------

## 🔐 Security Considerations

-   EC2 accessible only on required ports (80/22)
    
-   Application image versioned with Git SHA
    
-   Dependencies managed with Renovate
    
-   Secrets excluded using `.gitignore`
    

----------

## 🧠 What I Learned

-   How to write a GitHub Actions pipeline
    
-   How to deploy apps on EC2 via Docker Compose
    
-   How to integrate testing in CI
    
-   How to use Renovate for automatic dependency updates
    
-   How to simulate production-like conditions locally
    

----------

## 🛠️ Future Improvements

-   Add reverse proxy (Nginx) for production
    
-   Store secrets securely (e.g., AWS Secrets Manager)
    
-   Monitor the app with tools like Prometheus/Grafana
    
-   Extend the app with a database backend (e.g., PostgreSQL)
    
-   Add HTTPS (SSL) with Let's Encrypt or ACM
    

----------

## 📬 Contact

Made with ❤️ by **Mohamed-Rédha Bouras**  
[LinkedIn](https://linkedin.com/in/redhabouras) – [GitHub](https://github.com/redskot)  
Always open to collaboration and DevOps opportunities.

----------

## ✅ DevOps Learning Tracker

This project is part of my hands-on DevOps progression:

-   Dockerize a Flask app
    
-   Build CI/CD with GitHub Actions
    
-   Deploy to EC2 with Docker Compose
    
-   Add automated testing
    
-   Integrate Renovate for dependency updates
    
-   Add database & secrets management
    
-   Set up monitoring and alerting
    
-   Deploy to ECS or Kubernetes in the future
