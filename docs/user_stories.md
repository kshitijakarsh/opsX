# opsX — User Stories

## Overview

opsX is a multi-tenant project management and collaboration SaaS. These user stories capture the needs of different roles: Workspace Owner, Project Manager, and Contributor.

Each story follows the format:  
**As a [role], I want [action], so that [benefit].**

---

## Authentication & User Management

- As a User, I want to sign up with email and password so that I can create an account.  
- As a User, I want to log in securely so that I can access my workspace.  
- As a User, I want to reset my password via email so that I can recover my account.  
- As a User, I want to edit my profile (name, avatar) so that my team recognizes me.  
- As a User, I want to enable 2FA (future feature) so that my account is more secure.  

---

## Workspaces

- As a Workspace Owner, I want to create a workspace so that I can organize my projects.  
- As a Workspace Owner, I want to invite users via email so that my team can join.  
- As a Workspace Owner, I want to assign roles (admin, member) so that permissions are clear.  
- As a Workspace Owner, I want to remove users from the workspace so that I can control access.  
- As a Workspace Owner, I want to view a list of all members so that I can manage my team.  

---

## Projects

- As a Project Manager, I want to create a project inside a workspace so that I can track work.  
- As a Project Manager, I want to set project details (title, description, due date) so that the team knows the context.  
- As a Project Manager, I want to archive or delete projects so that old projects don’t clutter the workspace.  
- As a Contributor, I want to view a list of projects so that I can see where I belong.  

---

## Tasks

- As a Contributor, I want to create tasks inside a project so that I can track my work.  
- As a Contributor, I want to assign tasks to myself or teammates so that responsibility is clear.  
- As a Contributor, I want to update task details (title, description, status, priority, due date) so that progress is transparent.  
- As a Contributor, I want to move tasks between columns (To Do → In Progress → Done) so that work is visualized.  
- As a Contributor, I want to comment on tasks so that I can collaborate with teammates.  
- As a Contributor, I want to attach files to tasks so that relevant documents are accessible.  

---

## Real-Time Collaboration

- As a Contributor, I want to see task updates in real time so that I don’t need to refresh.  
- As a Contributor, I want to chat in a project channel so that we can discuss work quickly.  
- As a Contributor, I want to receive notifications when I’m assigned a task so that I don’t miss work.  

---

## Billing & Subscriptions

- As a Workspace Owner, I want to add a credit card and subscribe to a plan so that I can unlock premium features.  
- As a Workspace Owner, I want to see billing history so that I know what I’m paying for.  
- As a Workspace Owner, I want to upgrade or downgrade plans so that I can adjust to my team size.  
- As a Workspace Owner, I want a free plan with limits (e.g., 1 workspace, 5 members) so that I can try opsX before paying.  

---

## Security & Compliance

- As a Workspace Owner, I want to enforce role-based access control so that sensitive actions (billing, removing users) are restricted.  
- As a User, I want my password stored securely so that my data is safe.  
- As a User, I want my data to be private so that other workspaces cannot see it.  
- As a Workspace Owner, I want audit logs of user activity so that I can monitor workspace actions.  

---

## Admin & Settings

- As a Workspace Owner, I want to update workspace details (name, logo) so that it matches my team’s identity.  
- As a Workspace Owner, I want to deactivate a workspace so that unused workspaces don’t consume resources.  
- As a User, I want to manage my notification settings so that I only receive what’s relevant.  

---

## Extended Features (Future)

- As a Project Manager, I want Gantt chart views so that I can plan timelines.  
- As a Contributor, I want AI-powered task suggestions so that I can save time.  
- As a Workspace Owner, I want integrations (Slack, GitHub, Google Drive) so that opsX fits my existing workflow.