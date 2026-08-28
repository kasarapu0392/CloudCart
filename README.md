# CloudCart

CloudCart is a cloud-native full-stack e-commerce platform built to demonstrate production-style application development using **Golang, React, Docker, Kubernetes, and AWS**.

The application supports product browsing, user authentication, checkout, order management, inventory tracking, and background processing.

## Tech Stack

- **Backend:** Golang, REST APIs
- **Frontend:** React, TypeScript
- **Database:** PostgreSQL
- **Caching:** Redis
- **Containers:** Docker
- **Orchestration:** Kubernetes
- **Cloud:** AWS EKS, RDS, S3, ElastiCache, ALB, CloudWatch

## Architecture

```text
React Frontend
      |
      v
   Go API
      |
  +---+---+
  |       |
  v       v
Order   Inventory
Service  Service
   |
   v
Worker Service
   |
PostgreSQL + Redis

Docker
  |
Kubernetes
  |
AWS EKS
