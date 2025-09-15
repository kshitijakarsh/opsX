# opsX — Project Brief

## Project Overview

**Name:** opsX  
**Tagline:** Scalable project management and collaboration SaaS.  

**Description:**  
opsX is a web-based platform that helps small to mid-sized teams organize projects, manage tasks, and collaborate in real time. It provides workspaces, Kanban boards, chat, file sharing, and billing — all in one system designed to scale.

---

## Problem Statement

- Teams often use multiple disconnected tools (Slack for chat, Trello for boards, Drive for files, Stripe for billing).  
- This creates context switching, data silos, and integration pain.  
- Small teams want a single lightweight tool that grows with them.

---

## Goals & Objectives

- Build a multi-tenant SaaS that supports multiple workspaces and teams.  
- Provide MVP core features first: workspaces, projects, tasks, and real-time updates.  
- Add scalable add-ons: file uploads, chat, billing, audit logs.  
- Ensure production-grade quality: secure auth, RBAC, caching, monitoring, CI/CD.

---

## Target Users

- **Workspace Owner:** Creates workspace, invites team, manages billing.  
- **Project Manager:** Creates projects, assigns tasks, oversees progress.  
- **Contributor:** Works on tasks, comments, uploads attachments, chats.

---

## Key Features (MVP → Pro)

### MVP

- Authentication (signup/login, JWT sessions)  
- Workspace creation + invites  
- Projects & tasks (CRUD + Kanban board)  
- Role-based access (owner, admin, member)  
- Real-time task updates (WebSockets)

### Extended

- Comments & chat  
- File uploads (S3/Cloudinary)  
- Stripe subscription billing (free vs pro)  
- Notifications (email + in-app)  
- Audit logs (security & admin visibility)

---

## Success Metrics

- **Adoption:** User can create a workspace + first task within 5 minutes  
- **Engagement:** Daily active users (DAU) / Monthly active users (MAU) > 30%  
- **Conversion:** 10–20% of free workspaces upgrade to paid plan  
- **Reliability:** 99.9% uptime target for API + real-time services

---

## Constraints & Assumptions

### Tech Stack

- **Frontend:** Next.js 14 (App Router, server actions)  
- **Backend:** Next.js API routes (or Express service)  
- **Database:** PostgreSQL + Prisma ORM  
- **Cache / Queues:** Redis (caching, background jobs)  
- **Auth:** NextAuth (JWT + OAuth optional)  
- **Deployment:** Vercel (frontend), AWS/DigitalOcean (backend DB/Redis)

### Constraints

- Start with monolithic architecture (frontend + API together) → split later if needed  
- Optimize for developer velocity first, scaling later  
- Use existing SaaS infra (Stripe, S3, SendGrid) instead of building from scratch

---

## Timeline (Solo Dev Roadmap)

- **Phase 1 (2 weeks):** Planning → Brief, User Stories, Architecture, DB schema  
- **Phase 2 (3–4 weeks):** Core auth, workspaces, projects, tasks (MVP backend + frontend)  
- **Phase 3 (2–3 weeks):** Real-time updates, Kanban drag/drop, notifications  
- **Phase 4 (2 weeks):** File uploads, comments/chat  
- **Phase 5 (2–3 weeks):** Billing (Stripe), audit logs, admin dashboards  
- **Phase 6 (1 week):** CI/CD, deployment, monitoring, docs

---

## Deliverables

- **Codebase:** Next.js app + backend API + Prisma schema  
- **Docs:**  
  - User stories & requirements (`docs/user_stories.md`)  
  - ERD + architecture diagrams (`docs/architecture/*`)  
  - OpenAPI spec (`docs/openapi.yaml`)  
- **Deployment:** Live app (Vercel frontend + backend + Postgres/Redis)  
- **Demo:** Seeded demo workspace + landing page

---

## Risks & Mitigation

- **Scope creep →** stick to MVP → extended features later  
- **Scaling issues →** start monolith, add caching/queues before traffic grows  
- **Security gaps →** follow OWASP guidelines, test auth thoroughly  
- **DevOps complexity →** keep infra simple (Docker + Vercel + one cloud DB)

---

## Approval

**Prepared by:** [Your Name]  
**Date:** Sept 15, 2025  
**Status:** Draft v1
