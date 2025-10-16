# ✨ My Full-Stack ProDev Weekly Reflection

This week was a deep and exciting journey across the **full stack**, building and consuming **modern GraphQL APIs** using **Django**, **Next.js**, and **Apollo Client**. It tested my patience, sharpened my debugging skills, and reminded me how powerful precision and persistence can be.

---

## 🐘 Backend: Building a GraphQL API with Django

The backend challenge was to design a **CRM GraphQL API** from scratch.  
I set up a new Django project, integrated `graphene-django`, and created models for **Customers**, **Products**, and **Orders**. The core work involved defining **mutations** (like `createCustomer`, `bulkCreateCustomers`, and `createOrder`) and **queries** with advanced filtering using `django-filter`.

**💡 Biggest Lesson:**  
A failing automated checker had me troubleshooting for hours until I discovered the issue was a **naming mismatch** in my project folder. That tiny fix taught me how crucial it is to **follow project specs to the letter**.

---

## 👨‍🚀 Frontend: Consuming GraphQL with Next.js + React

On the frontend, I explored how to fetch and display live data using **Apollo Client** and the **Rick and Morty GraphQL API**.  
I started by writing raw GraphQL queries in the playground, then built a **Next.js + TypeScript** app that used the `useQuery` hook to fetch and paginate episode data with a clean **Tailwind CSS** layout.

**⚙️ Challenge:**  
I encountered a stubborn runtime error — `useQuery is not a function` — after duplicating my project structure. It revealed how tricky **dependency management and caching** can be in JavaScript projects. Though the automated checker passed, it reminded me that **real runtime debugging** is a different kind of test.

---

## 🏆 Achievement Highlight

I proudly ranked **#3 on the ProDev Backend Track Leaderboard (Month 2)** 🎉

<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/ProDev%20BE%20Leaderboard.jpg" alt="Leaderboard" width="400">

---

## 🛠️ Tech Stack & Tools Used

**Backend:**  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

**Frontend:**  
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Apollo Client](https://img.shields.io/badge/Apollo_Client-311C87?style=for-the-badge&logo=apollographql&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

✨ *This week pushed me to think like both a backend engineer and a frontend architect, connecting logic with design, structure with flow, and code with clarity. Every bug, every rename, every ‘aha!’ moment added another layer to my full-stack confidence.* 🚀
