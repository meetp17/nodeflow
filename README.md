# Nodeflow

Nodeflow is a simplified container management system inspired by Kubernetes.
It is designed to automate container deployment, monitoring, restarts, and
basic traffic routing across machines.

This project focuses on understanding how container orchestration systems
work internally by building a smaller and more approachable version.

---

## Why Nodeflow?
Managing containers manually becomes difficult as applications scale.
Containers may crash, traffic may spike, and recovery often requires manual
intervention. Nodeflow aims to reduce this manual effort through automation.

---

## Features
- Container lifecycle management
- Health checks and automatic restarts
- Basic scheduling
- Simple HTTP load balancing
- Central controller with node agents

---

## Tech Stack
- Node.js
- JavaScript
- Docker
- Express.js
- Dockerode

---

## Project Status
📄 Proposal and system design completed  

---

## Inspiration
This project is inspired by Kubernetes but intentionally keeps the system
simple and lightweight for learning purposes.
