# Nodeflow – Container Management System

## Overview
Nodeflow is a simplified container management system inspired by Kubernetes.
When applications run in multiple containers, manual management becomes
difficult. Containers may crash, traffic may increase, and keeping everything
running smoothly across machines is challenging.

Nodeflow introduces a central controller, small agents on each machine, and
a basic scheduler to automate container deployment, monitoring, and recovery.
A simple load balancer helps distribute incoming traffic evenly. The goal is
to make container management easier, more reliable, and less manual.

---

## User Flow
1. User provides a simple configuration
2. User enters application name
3. User selects a container image
4. Each instance shows its status (starting/running)
5. User sees real-time health updates
6. System auto-recovers from failures
7. User accesses the app via a single URL
8. User can monitor the application anytime

---

## Tech Stack
- Node.js – main system components
- JavaScript – core logic and communication
- Docker – container runtime
- Express.js – APIs between controller and agents
- Dockerode – programmatic Docker control
- HTTP / REST APIs – communication
- Node.js HTTP Proxy – basic load balancing

---

## APIs Used
### Docker API (via Dockerode)
Used to start, stop, inspect, and manage containers.

### HTTP Proxy API (Load Balancer)
Used to forward user traffic to the correct running container.

---

## Edge Cases & Limitations
- No rolling updates or version control
- No horizontal or vertical auto-scaling
- No fault tolerance for the controller

These limitations are acknowledged and kept intentionally to maintain system
simplicity.

---

## Current Status
Proposal and system design completed.
