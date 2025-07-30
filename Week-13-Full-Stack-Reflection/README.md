# 💡 Weekly Reflection: Full-Stack Progress (ALX Frontend + Backend)

## 🔥 Overview
This week was packed with new skills and real victories across both **frontend** and **backend** engineering. From setting up a GitHub user search app with React + Tailwind to building my first fully authenticated API with Django REST Framework, I've officially crossed over into full-stack mode!

---

## 🎨 Frontend 

### ✅ Tasks Completed
- **Project Setup**
  - Initialized Vite + React app
  - Set up Tailwind CSS with PostCSS
  - Created a clean folder structure for the `github-user-search` app

- **Search Form**
  - Implemented inputs for:
    - `username`
    - `location`
    - `min_repos`
  - Added state management with React's `useState`

- **API Integration**
  - Fetched user data from the GitHub API using `fetchUserData`
  - Displayed results with basic styling

- **Deployment**
  - Pushed project to GitHub
  - Successfully deployed to **Vercel**:
    🔗 [Live Site](https://alx-fe-reactjs-git-main-matilda-esenam-gbeves-projects.vercel.app/)

- **Environment Security**
  - Ensured `.env` file is ignored in Git and not committed
  - Passed all project checks including environment safety 🎯

---

### 🧠 Key Learnings
- Working with **Tailwind** inside a React app using PostCSS
- Managing environment variables securely in frontend projects
- Structuring components and state in React
- Debugging build errors during local dev and deployment

---

## 🐍 Backend (Django REST API Module)

### ✅ Tasks Completed

#### 1. **API Project Setup**
- Created a new folder `api_project` inside my main Django repo (`Alx_DjangoLearnLab`)
- Initialized a new Django project and app (`api`)

#### 2. **My First API Endpoint**
- Built a `/api/books/` endpoint
- Used Django REST Framework to return serialized JSON responses

#### 3. **CRUD with ViewSets and Routers**
- Replaced function-based views with:
  - `ModelViewSet` for full CRUD (Create, Read, Update, Delete)
  - `DefaultRouter` for automatic URL routing

#### 4. **Token Authentication + Permissions**
- Enabled token-based auth in `settings.py`
- Installed and configured `rest_framework.authtoken`
- Added permission classes to secure endpoints
- Tested authenticated routes with tokens

---

### 🧠 Key Learnings
- REST API development using Django REST Framework
- ViewSets and Routers for faster API scaffolding
- Token authentication for securing APIs
- Structuring Django apps modularly within a shared repo

---

## 🚀 Reflections & Wins
This week proved I'm mastering the flow between **frontend form inputs**, **API integration**, and **backend logic**. I deployed a full React app, consumed an external API, and built my own with authentication from scratch.

I can boldly say I'm not just building, I'm **engineering**.

---

## Some Screenshots
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Github%20User%20Search.png" alt="FE" width="350">
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/GUS%20App.png" alt="GUS App" width="350">
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Django%20REST%20Framework.png" alt="BE" width="350">
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Vercel%20deployment.png" alt="Vercel" width="350">
---

## 📅 Next Steps
- Enhance the UI for your GitHub search app with cards or avatars
- Add pagination or filters to my DRF API
- Learn how to consume my **own backend** with React frontend (full integration!)
