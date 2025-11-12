# Linux Setup and Configuration Guide for a DevOps Practice Lab

## Overview
This guide provides clear, step-by-step instructions for setting up a **Linux environment** for DevOps learning and experimentation.  
It is designed for beginners who want to get hands-on experience with **Linux commands, shell scripting, Git, Docker, and CI/CD basics**.

> **Author:** Miracle Chisom Ikechukwu  
> **GitHub:** [Chisney25](https://github.com/Chisney25)  
> **Last Updated:** November 2025  

---

## Objectives
By following this guide, you will learn how to:
- Install and configure Linux (Ubuntu/Debian-based)
- Navigate the Linux file system and use basic commands
- Manage users and permissions
- Install essential DevOps tools (Git, Docker)
- Use Markdown for documentation
- Set up Git for version control and connect to GitHub

---

## 1. System Requirements
| Component | Minimum Requirement | Recommended |
|------------|--------------------|--------------|
| OS | Ubuntu 22.04 LTS (or Debian-based distro) | Ubuntu 24.04 LTS |
| RAM | 4 GB | 8 GB |
| Disk Space | 25 GB | 50 GB |
| Internet | Required | Stable broadband |

---

## 2. Installing Linux (Ubuntu Example)
You can install Linux in three ways:

### Option 1: Virtual Machine (Recommended)
1. Download **[VirtualBox](https://www.virtualbox.org/)** or **VMware Workstation Player**.
2. Download **Ubuntu ISO** from [ubuntu.com/download](https://ubuntu.com/download).
3. Create a new VM:
   - 4 GB RAM  
   - 25 GB Disk  
   - Network: Bridged Adapter  
4. Boot and follow installation prompts.

### Option 2: Dual Boot
Install Ubuntu alongside Windows (advanced users).

### Option 3: Cloud Instance
Use a free-tier cloud VM (e.g., **AWS EC2**, **Azure**, or **Google Cloud Compute Engine**).

---

## 3. Basic Linux Commands
Here are essential commands every DevOps engineer should know:

| Command | Description |
|----------|-------------|
| `pwd` | Print current working directory |
| `ls -l` | List files with details |
| `cd /path` | Change directory |
| `cp source target` | Copy files or directories |
| `mv old new` | Move or rename files |
| `cat file.txt` | Display file content |
| `grep pattern file.txt` | Search inside files |
| `chmod 755 file.sh` | Change permissions |
| `sudo apt update && sudo apt upgrade` | Update system packages |

> *Tip:* Always use `man <command>` to read the manual for any command.

---

## 4. Managing Users & Permissions
Create a new user:
```bash
sudo adduser devopsuser
sudo usermod -aG sudo devopsuser
```

---

## 5. Installing Git and Configuring GitHub
Install Git:
sudo apt install git -y

Set global configuration:
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"

Generate and add SSH key to GitHub:
ssh-keygen -t ed25519 -C "youremail@example.com"
cat ~/.ssh/id_ed25519.pub
Then add the key at GitHub → Settings → SSH and GPG keys → New SSH Key.

---

## 6. Practice: Creating Your First Markdown Documentation
Create a simple README in Markdown:
mkdir docs && cd docs
nano README.md
Paste the following:
# My First Documentation Project
This is a Markdown example created on Linux.
Save and exit (Ctrl + O, Ctrl + X).

---

## 7. Pushing to GitHub
git init
git add .
git commit -m "Initial commit: Linux setup documentation"
git branch -M main
git remote add origin git@github.com:Chisney25/linux-devops-lab-guide.git
git push -u origin main

---

## 8. Contributing
This is an open documentation project — feedback, edits, and suggestions are welcome.
To contribute:
1. Fork the repository.
2. Make edits and test Markdown locally.
3. Submit a pull request with a short description.

---

## 9. License
This project is licensed under the MIT License — free to use and modify with attribution.

---

## Summary
By completing this guide, you will:
1. Understand the basics of Linux navigation and file permissions.
2. Be able to document your own DevOps experiments.
3. Use Git and Markdown for open-source collaboration.

---









