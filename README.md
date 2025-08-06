# 100 Days of DevOps Practice

**A collection of Linux administration and DevOps practices.**

This repository tracks my progress and hands-on experience as I work through the **100 Days of DevOps** challenge. Each day is focused on building real-world DevOps skills in small, manageable tasks that take about 1 hour.

---

## Challenge Overview

The **100 Days of DevOps** is a practical challenge aimed at learning by doing. The tasks cover:

- Linux System Administration  
- Docker & Kubernetes  
- Git & Version Control  
- Continuous Integration / Continuous Deployment (CI/CD)  
- Infrastructure as Code (IaC)

---

## Day 1 - Linux User Setup with a Non-Interactive Shell

**Objective**: Create a user with no interactive shell access to enhance system security.

- Created a new system user `webdeploy`
- Set the shell to `/usr/sbin/nologin`
- Ensured user can't log in interactively but can perform system tasks like deployments

---

##  Custom Apache Server Setup

**Objective**: Set up a basic custom Apache HTTP server to serve a webpage.

- Installed Apache web server
- Changed the default document root
- Hosted a custom HTML file
- Verified that the Apache server runs and displays the custom content

---

## Create Group Across Servers and Add User to Group

**Objective**: Centralize permissions by creating a shared group and adding users across multiple servers.

- Created a group `nautilus_admin_users`
- Added existing user `jarod` to the `nautilus_admin_users` group
- Applied consistent group permissions on shared directories across two or more servers

---
## Day 2: Temporary User Setup with Expiry



##  Notes

This journey is based on the 100 Days of DevOps challenge, which encourages:

> *“Hands-on daily challenges to learn DevOps by doing.”*

---
