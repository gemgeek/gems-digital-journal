# 🌍 **Full-Stack ProDev Weekly Reflection**

> _"Building from backend containers to frontend polish — a true full-stack growth week!"_ ✨



## 🖥️ **Backend Summary — Containerization with Docker**

This week’s backend focus was all about **containerizing a Django application** using **Docker** 🐳.  

### 🧱 Key Highlights:
- Set up a **professional development environment** on **Windows** using **WSL 2 + Ubuntu**.  
- Wrote a **Dockerfile** to create a portable image of the Django app.  
- Configured a **docker-compose.yml** to orchestrate a **multi-container setup**, linking:
  - 🐍 **Django App**
  - 🗄️ **MySQL Database**
- Debugged and solved several key issues:
  - Missing system dependencies for Python packages like `mysqlclient`.  
  - Python package errors and dependency conflicts during Docker build.  
  - Network port conflicts between Docker and the local machine.

🎉 **Result:**  
A fully functional, multi-container Django + MySQL setup that runs smoothly with a single command:
```
docker-compose up
```
---

## 🎬 **Frontend Summary — Building the “CineSeek” Movie App**

On the frontend, I started building a **movie discovery app** called **CineSeek** 🍿 using modern web technologies.

### 🪄 Tech Stack:
| Tool | Badge |
|------|--------|
| **Next.js** | [![Next.js](https://img.shields.io/badge/Next.js-black?logo=next.js&logoColor=white)](https://nextjs.org/) |
| **TypeScript** | [![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/) |
| **Tailwind CSS** | [![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/) |
| **MoviesDatabase API** | [![API](https://img.shields.io/badge/API-RapidAPI-blue?logo=rapidapi&logoColor=white)](https://rapidapi.com/) |

---

### 🧩 Development Highlights:
- Analyzed the **MoviesDatabase API** and created a detailed `README.md` outlining the project’s plan.  
- Bootstrapped a clean, component-based **Next.js + TypeScript** structure.  
- Developed reusable UI components like:
  - 🧭 Header  
  - 🎞️ MovieCard  
  - 🔘 Button  
  - ⚓ Footer  
- Built a **secure Next.js API route** (`/api/fetch-movies`) to handle all API communication — keeping API keys safe.
- Implemented the `/movies` page with:
  - 🎛️ State management for **filters** (year, genre)
  - 🔄 **Pagination**
- Debugged:
  - 403 Forbidden errors (API key & subscription issues)
  - Next.js **external image configuration** for secure rendering.

💅 **Result:**  
A beautifully styled, functional movie browsing page built from scratch with clean UI and robust API integration.

<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_10-10-2025_12401_localhost.jpeg" alt="Screenshot" width="350">
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_10-10-2025_131450_localhost.jpeg" alt="Screenshot" width="350">
---

## 🚀 **Reflection**

This week tested both my backend and frontend engineering skills.  
From orchestrating Docker containers 🧩 to crafting interactive Next.js components 💻 —  
it was a **hands-on, full-stack learning experience** that strengthened my problem-solving, debugging, and system design mindset.

---

### 🧰 **Tech Tools Used**
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)  
[![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)](https://www.djangoproject.com/)  
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)  
[![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white)](https://ubuntu.com/)  
[![WSL2](https://img.shields.io/badge/WSL2-4D4D4D?logo=windows&logoColor=white)](https://learn.microsoft.com/en-us/windows/wsl/)  

---

✨ **End of Reflection — onwards to the next sprint!**
