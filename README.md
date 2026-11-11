# Mental Health Assessment SaaS (Genesis for Health) — Case Study

> Multi-tenant SaaS I designed and built for **Genesis for Health** to run mental health assessments.
> **Source code is private.** This repository documents the project; a live walkthrough is available on request.

![React](https://img.shields.io/badge/React-149ECA?logo=react&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![Express](https://img.shields.io/badge/Express-000?logo=express)
![Drizzle](https://img.shields.io/badge/Drizzle_ORM-C5F74F?logo=drizzle&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white)

## What it does

- **Multi-tenant** platform: each organization manages its own users, patients and assessments with isolated data.
- Applies and scores **mental health assessments** and keeps the history for follow-up.
- Built with sensitive health data in mind: access control per tenant and per role.

## Architecture

```mermaid
flowchart LR
  B[Browser<br/>React + Vite SPA] --> N[Nginx] --> A[Express API]
  A --> D[(PostgreSQL<br/>Drizzle ORM)]
```

- React + Vite front end, Express API, Drizzle ORM on PostgreSQL.
- **Self-hosted** on a VPS behind Nginx (TLS, reverse proxy), keeping infrastructure cost low.

## My role

Architecture, data modeling, full stack development, deployment and infrastructure.

---
Built by **Victor Sestrem** · [LinkedIn](https://www.linkedin.com/in/victor-sestrem/) · victor-sestrem@hotmail.com
