# 📖 My Full-Stack Weekly Reflection 🚀

This week was a solid journey across frontend, backend, and shell scripting. I tackled four major areas: **React state management, responsive UI, Django signals, API optimization, and shell scripting with variables and expansions**.

---

## 🎨 Frontend Reflection: State & Responsive Design

### 🧮 Assignment 1: Counter App (State Management)
We rebuilt the same app three times to explore different state management techniques:
- **useState Hook** – simple for local state, but limited to single components.
- **Context API** – introduced shared global state via a `CountProvider` and `useCount` hook.
- **Redux Toolkit** – robust and scalable with `store`, `slice`, `useSelector`, and `useDispatch`. Ideal for large apps.

### 🏡 Assignment 2: Property Listing App
Focused on real-world UI development:
- **Dynamic Routing**: Used `[id].tsx` for property pages in Next.js.
- **Component Composition**: Built reusable pieces like `BookingSection` and `ReviewSection`.
- **Responsive Design**: Tailwind’s responsive classes (`md:`, `lg:`) made layouts adapt smoothly.
- **Typed Data**: Defined strong TypeScript interfaces and mock data for realism.

📸

<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_2-10-2025_10430_localhost.jpeg" alt="SplashApp1" width="350">
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_2-10-2025_104259_localhost.jpeg" alt="SplashApp2" width="350">


**Frontend Tech Stack**:  
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) 
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white) 
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white) 
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white) 
![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white) 
![React Icons](https://img.shields.io/badge/React_Icons-E91E63?style=for-the-badge&logo=react&logoColor=white)    

---

## 🚀 Backend Reflection: Signals & APIs

### 📡 Django Signals & ORM Optimization
- **post_save**: Auto-created `Notification` when a new `Message` was saved.  
- **pre_save**: Logged edits to `MessageHistory`.  
- **post_delete**: Cleaned up messages when a user was deleted.  
- **ORM Optimization**: Solved N+1 queries with `select_related` & `prefetch_related`.  
- **Custom Manager**: `UnreadMessagesManager` made querying cleaner.  
- **Caching**: Used `@cache_page(60)` to reduce DB load.

### ✈️ Travel App API (Django REST Framework)
- **ModelViewSet & Routers**: Delivered full CRUD for `Listing` and `Booking` with minimal code.  
- Felt like a true productivity boost ⚡.

## 🐚 Shell Scripting Reflection: Variables & Expansions

This week I also worked on **ALX Shell Variables and Expansions**.  
I wrote Bash scripts to practice key shell concepts:

- **Variables**: Creating local and global variables using `set` and `export`.  
- **Expansions**: Arithmetic (`$((...))`), brace expansions, and alias creation.  
- **Text Processing**: Using commands like `tr`, `grep`, `cut`, and `printf`.  
- **Base Conversion & ROT13**: Solving puzzles like binary → decimal, decimal → hex, and text encoding.  
- **File Permissions**: Remembering to `chmod +x` scripts for execution.  

This gave me hands-on experience with **Linux shell scripting, environment management, and text manipulation**.

**Shell Tools Used**:  
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white) 
![VS Code](https://img.shields.io/badge/VS_Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white) 
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) 
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white) 

---

## 🧩 Key Learnings & Challenges
- Major issue: **persistent `ModuleNotFoundError`** caused by environment corruption.  
- Solution: **hard reset** (delete venv, caches, migrations) → rebuild step by step.  
- Lesson: sometimes debugging is about fixing the environment, not the code.

---

**Backend Tech Stack**:  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white) 
![Django REST](https://img.shields.io/badge/Django_REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=gray) 
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) 
![VS Code](https://img.shields.io/badge/VS_Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white) 
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) 
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white) 
 
