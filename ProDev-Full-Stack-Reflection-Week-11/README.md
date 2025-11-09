# 🌸 ProDev Weekly Reflection  
---

## 🚀 Backend Assignment 1: Security & IP Tracking System  

**Tech Stack Badges:**  
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)  
![Celery](https://img.shields.io/badge/Celery-37814A?logo=celery&logoColor=white)  
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)  
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)  
![REST API](https://img.shields.io/badge/REST-005571?logo=fastapi&logoColor=white)  
![ipinfo](https://img.shields.io/badge/ipinfo-1F73B7?logo=ipinfo&logoColor=white)  
![Security](https://img.shields.io/badge/Security-000000?logo=security&logoColor=white)

This week, I engineered a **full security and monitoring system** for production-grade Django apps.

### ✅ Key Features
- **Middleware Logging** using django-ipware for accurate client IPs  
- **Geolocation** with ipinfo API + 24hr caching  
- **IP Blacklisting** with automatic 403 blocks  
- **Rate Limiting** for anonymous vs authenticated users  
- **Celery Beat Anomaly Detection** scanning logs hourly for suspicious activity

---

## 🚀 Backend Assignment 2: Deploying the Django “Travel App”  

**Tech Stack Badges:**  
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)  
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?logo=gunicorn&logoColor=white)  
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?logo=rabbitmq&logoColor=white)  
![Celery](https://img.shields.io/badge/Celery-37814A?logo=celery&logoColor=white)  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)  
![Render](https://img.shields.io/badge/Render-46E3B7?logo=render&logoColor=white)  
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?logo=swagger&logoColor=black)

This assignment focused on **full production deployment** using Render.

### ✅ Highlights
- Web service + background worker  
- CloudAMQP (RabbitMQ) integration  
- Gunicorn setup for production  
- Swagger API docs at `/swagger/`  
- Secured all environment variables  
- Proper Procfile for Render deployment  

### 🛠 Major Fixes
- Python version mismatch fixed with `PYTHON_VERSION=3.10.11`  
- Backport dependency conflict fixed by upgrading `asgiref`  

---

## 🖥️ Frontend Assignment: Deploying the Next.js “Listing App”  

**Tech Stack Badges:**  
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)  
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)  
![Axios](https://img.shields.io/badge/Axios-5A29E4?logo=axios&logoColor=white)  
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)  
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)

This was a **deep debugging and deployment journey** on Vercel.

### ✅ Key Fixes
- ESLint errors fixed with proper typing (`unknown` instead of `any`)  
- Added `getServerSideProps` to fix static build issues  
- Solved ETIMEDOUT by switching to `VERCEL_URL` in SSR  
- Disabled unwanted Vercel Authentication (was blocking API calls)  
- Fixed routing typo that broke property card clicks  

### ✅ Final Outcome
Fully deployed, dynamic, SSR-powered listing app with working images, reviews, and property details.

---

## 🏆 Achievement of the Week  
### 🥇 **Ranked #1 on the ProDev Backend Leaderboard for the Month**  
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/prodev%20m3.jpg" alt="ProDev" width="400">

---

> Another powerful week of problem-solving, debugging, deployment mastery, and backend brilliance. GEM GEEK is unstoppable. 🚀✨
