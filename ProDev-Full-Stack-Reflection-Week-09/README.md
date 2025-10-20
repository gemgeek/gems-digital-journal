# ✨ Full-Stack Weekly Reflection 💻🌸🧠

<div align="center">

🎯 **Tech Stack & Tools**  
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D33833?style=for-the-badge&logo=jenkins&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

</div>

---

## 🌐 FRONTEND

This week was a **power move**! I tackled bugs head-on and completed **two major frontend projects** that leveled up both my technical and debugging confidence. 🚀  

### ⚡ Project 1: React Error Handling (Error Boundaries + Sentry)
I built a resilient error-handling system to prevent the dreaded white screen of death.  
- Created an `ErrorBoundary.tsx` class component to catch UI crashes using lifecycle methods like `getDerivedStateFromError`.  
- Wrapped the entire app in `<ErrorBoundary>` for global protection.  
- Integrated **Sentry** for real-time error monitoring, every crash now sends detailed logs to my dashboard.  
- Debugged missing imports and dependencies that were breaking builds.  

💡 *Result:* My React app is now production-ready, stable, and observable.  

---

### 🌍 Project 2: Progressive Web App (PWA) Conversion
I transformed my **Cine Seek** movie website into an **installable PWA** that works offline, like a real mobile app!  
- Added caching, a service worker, and app manifest with **next-pwa**.  
- Customized `manifest.json`, defined icons, and connected it via `_document.tsx`.  
- Verified functionality through Chrome DevTools and deployed to **Vercel** using the CLI.  

💡 *Result:* The app can now be installed on phones and desktops, fully offline capable and blazing fast.  

---

## ⚙️ BACKEND

This section was all about **automation, DevOps, and CI/CD**,  the invisible magic that keeps apps alive and scalable. 💪  

### 🧩 Jenkins CI/CD Pipeline
I set up a local **Jenkins server in Docker**, securing credentials for GitHub and Docker Hub.  
- Defined a complete build flow in a `Jenkinsfile`: clone repo → install dependencies → run tests → build image → push to Docker Hub.  
- Used volumes to preserve Jenkins data and credentials.  
- Debugged ShiningPanda plugin syntax and static checker mismatches.  

💡 *Result:* I automated the backend build and deployment process end-to-end.  

---

### ☁️ GitHub Actions Workflow
I implemented **two workflows** under `.github/workflows`:  

- **`ci.yml`** → Handles testing, linting, and coverage reports.  
- **`dep.yml`** → Builds and deploys Docker images automatically after tests pass.  

Key learnings:  
- Set up a MySQL service for testing.  
- Used GitHub Secrets for Docker Hub authentication.  
- Discovered that workflows must sit in `.github/workflows` to trigger correctly.  

💡 *Result:* My Django app now has cloud-based CI/CD automation, every push triggers tests and deployments like a pro-grade DevOps setup.  

---

### 🌈 Reflection
This week, I felt like a **true full-stack engineer** — balancing front-end aesthetics with back-end reliability.  
I learned that debugging is not failure; it’s refinement. Every “why is this breaking?” moment became a “now I know how it works.”  

✨ From Sentry alerts to Jenkins builds, from Next.js service workers to Docker pushes, everything connected.  
I didn’t just build apps; I built **systems that sustain apps**.  

---

🪩 **Next Focus:**  
> Polish my UI design flow with animations & continue exploring cloud orchestration (Kubernetes) for production-level scaling.  

💖 *Signed*  
