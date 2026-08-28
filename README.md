# DevConnect 🚀

DevConnect is a Node.js/Express backend application connected to MongoDB Atlas and deployed using Docker and Kubernetes.

This project demonstrates how a backend application can be containerized, deployed, exposed, monitored, scaled, updated, and rolled back using Kubernetes.

---

## 📌 Project Overview

The main goal of this project is to take a backend application and deploy it using a production-style Kubernetes architecture.

The project covers:

- Node.js and Express backend
- MongoDB Atlas
- Docker containerization
- Kubernetes Deployments
- ReplicaSets
- Pods
- Kubernetes Services
- NGINX Ingress
- ConfigMaps
- Secrets
- PersistentVolumeClaims
- Readiness Probes
- Liveness Probes
- CPU and memory requests and limits
- Horizontal Pod Autoscaler (HPA)
- Manual scaling
- Rolling Updates
- Rollbacks

---

## 🛠️ Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose

### DevOps / Deployment
- Docker
- Kubernetes
- NGINX Ingress Controller
- Kubernetes Metrics Server

---

## 🏗️ Architecture

```text
                              User / Client
                                   │
                                   ▼
                         NGINX Ingress Controller
                                   │
                                   ▼
                            Ingress Rules
                                   │
                                   ▼
                    devconnect-backend-service
                                   │
                       ┌───────────┴───────────┐
                       ▼                       ▼
                    Backend Pod             Backend Pod
                       │                       │
                       ▼                       ▼
                    Container               Container
                       │                       │
                       ▼                       ▼
                 Node.js / Express       Node.js / Express
                       │                       │
                       └───────────┬───────────┘
                                   ▼
                             MongoDB Atlas




⭐ Project Highlights

Docker
   ↓
Kubernetes
   ↓
Deployment
   ↓
ReplicaSet
   ↓
Pods
   ↓
Service
   ↓
Ingress
   ↓
Health Checks
   ↓
Resource Management
   ↓
HPA
   ↓
Rolling Updates
   ↓
Rollback