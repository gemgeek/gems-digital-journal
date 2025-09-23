# 🚀 ProDev Full-Stack: Weekly Reflection 🌟

This week in Backend was a deep dive into building and securing a real-world backend application with Django. We tackled two major projects, going from basic API construction to advanced concepts like middleware and debugging complex issues.

---

## Assignment 1: Building a Robust Messaging API 💬

Our first goal was to create a secure and functional messaging API using Django REST Framework.

### 🛡️ Task 1: Implementing JWT Authentication
We started by setting up the core of our security system.
- Installed `djangorestframework-simplejwt` to handle token-based authentication.
- Configured `settings.py` by adding the new apps and setting up the `REST_FRAMEWORK` defaults.
- Set up the `/api/token/` and `/api/token/refresh/` endpoints in `urls.py`.

### 🔐 Task 2: Custom Permissions
With users logging in, we needed to control what they could access.
- Created a custom permission class, `IsParticipantOfConversation`, to ensure users could only interact with conversations they were a part of.
- Applied this permission to our `ConversationViewSet`.
- Set a global default permission (`IsAuthenticated`) in `settings.py` as a security best practice.

### 📄 Task 3: Pagination & Filtering
To handle large amounts of data efficiently, we added pagination and filtering.
- Installed `django-filter` to enable powerful query filtering.
- Created a custom `MessagePagination` class to serve 20 messages per page.
- Built a `MessageFilter` class to allow filtering messages by `sender` and `timestamp`.

### 🧪 Task 4: API Testing with Postman 📮
We verified that everything worked as expected using Postman.
- Created a collection to organize all our API requests.
- Set up requests to get a JWT token, create conversations, fetch conversations, and send messages.
- A key learning was using Postman's scripting features to automatically save the JWT `accessToken` to a collection variable for use in subsequent requests.

### 🛠️ Key Debugging Moments (Assignment 1)
- **Database Initialization:** We encountered `no such table` and `InconsistentMigrationHistory` errors, which taught us the importance of the `makemigrations` -> `migrate` -> `createsuperuser` workflow, especially after creating a custom user model or resetting the database.
- **Custom User Model:** We fixed an `AttributeError: 'User' object has no attribute 'id'` by correctly configuring `SIMPLE_JWT` in `settings.py` to use our custom primary key (`user_id`).
- **Django Admin:** We learned that custom models must be registered in `admin.py` to appear in the admin panel and how to use `UserAdmin` to make the interface more powerful.

---

## Assignment 2: Mastering Django Middleware 🌉

The second project focused on intercepting and processing requests using middleware, a powerful tool for cross-cutting concerns.

### 📝 Task 2: Request Logging Middleware
- Created our first middleware, `RequestLoggingMiddleware`, to log the timestamp, user, and path of every incoming request to a `requests.log` file.

### ⏰ Task 3: Time-Based Access Control
- Implemented `RestrictAccessByTimeMiddleware` to return a `403 Forbidden` error if a user tried to access the app outside of business hours (9 AM - 6 PM).

### 🚦 Task 4: IP-Based Rate Limiting
- Built a middleware (named `OffensiveLanguageMiddleware` as per the prompt) that cleverly tracked the number of `POST` requests from each IP address, blocking them if they exceeded 5 messages per minute. This was a great introduction to stateful middleware.

### 👑 Task 5: Role-Based Permissions
- Created `RolePermissionMiddleware` to check the `user.role` attribute and deny access to users who weren't 'ADMIN' or 'HOST'.

### 🐛 The Great Checker Showdown (A Debugging Saga)
A significant part of this assignment was battling a buggy automated checker. This was a valuable, real-world lesson in debugging.
- We learned that error messages can be misleading (`settings.py doesn't exist`).
- We tried multiple valid project structures (`config` folder, matching project name folder).
- Ultimately, we discovered the solution was to **flatten the project structure**, moving the settings files to the project root. This taught a valuable lesson: sometimes the problem isn't the code, but the environment or the tools used to check it. Your persistence and debugging here were awesome! 🎉

---

### 💻 Tech Stack & Tools Used
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
- ![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
- ![Django REST Framework](https://img.shields.io/badge/Django%20REST-A30000?style=for-the-badge&logo=django&logoColor=white)
- ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
- ![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
- ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
- ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

# 🎨 My Frontend Reflection

This week was a hands-on experience building two full-stack web applications, focusing on modern frontend technologies. The goal was to master the fundamentals of **Next.js**, **TypeScript**, and **Tailwind CSS** by building reusable components, managing state, handling routing, and interacting with APIs.

---

## 🚀 Project 1: Next.js Fundamentals (`alx-project-0x02`)

This project was a deep dive into the core concepts of building a structured and dynamic web application from the ground up.

### 🏗️ Scaffolding & Setup
We began by setting up a professional development environment.
- Initialized a new Next.js project using the **Pages Router**.
- Manually installed and configured **Tailwind CSS v3** to have precise control over the styling library.
- Integrated **TypeScript** and **ESLint** from the start for a robust, type-safe, and clean codebase.

### 🧩 Building Reusable Components
A major focus was on component-based architecture.
- **`Card` & `Button`:** Created foundational, reusable components that accept props for dynamic content and styling (`size`, `shape`). This taught me about conditional styling and TypeScript `interface` design using union types (`'small' | 'medium'`).
- **`PostCard` & `UserCard`:** Built more specific components to display data fetched from an external API.

### 🔄 State Management & Interactivity
We brought the application to life with state and user interaction.
- **`PostModal`:** Implemented a modal component to create new posts.
- **`useState` Hook:** Learned to use React's `useState` hook to manage the modal's visibility and to dynamically update a list of posts on the page without a browser refresh.
- **Passing Functions as Props:** Mastered the pattern of passing callback functions (`onClose`, `onSubmit`) from a parent page to a child component to enable communication.

### 🌐 API Data Fetching
We connected our frontend to the outside world by fetching data.
- **`getStaticProps`:** Used Next.js's powerful data fetching method to pull post and user data from the JSONPlaceholder API at build time, ensuring a fast and SEO-friendly user experience.
- **TypeScript Interfaces:** Created detailed interfaces (`Post`, `User`, `Address`) to accurately model the nested JSON data returned from the API, preventing runtime errors.

---

## ✨ Project 2: Splash App - Layouts, Fonts & UX (`alx-project-0x03`)

This project built on the first by focusing on creating a polished, professional user experience with a focus on code organization and reusability (DRY principle).

### 🏛️ The DRY Principle: Shared Layouts
We created a consistent look and feel across the entire application.
- Built a reusable `Layout` component that included a shared `Header` and `Footer`.
- Applied this layout globally to all pages using the special **`pages/_app.tsx`** file, ensuring that any page created would automatically have the correct header and footer.

### ✍️ Custom Fonts & Styling
We customized the app's typography for a unique brand identity.
- Integrated **Google Fonts** by importing the 'Montserrat' font directly into the `styles/globals.css` file.
- Applied the font globally to the `body` element.

### 🗺️ Imperative vs. Declarative Routing
We explored two different ways to handle navigation.
- **Declarative:** Used the standard `<Link>` component for static navigation in the header.
- **Imperative:** Implemented navigation from button clicks using the `useRouter` hook from `next/router`. This allowed us to programmatically "push" users to new pages after an action occurred.

### 👻 Custom Error Handling
We improved the user experience for non-existent pages.
- Created a custom, beautifully styled 404 page by creating a **`pages/404.tsx`** file, leveraging a core Next.js feature.

---

### 📸 My Work in Action!

Here are some screenshots of the final "Splash App" project.

#### Main Landing Page
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_23-9-2025_222356_localhost.jpeg" alt="Landing Page">

#### Custom 404 toning
<img src="https://github.com/gemgeek/gems-digital-journal/blob/main/assets/Screenshot_23-9-2025_2343_localhost.jpeg" alt="404">

---

### 💻 Technologies & Tools Used
- ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
- ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
- ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
- ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
- ![React Icons](https://img.shields.io/badge/React_Icons-E91E63?style=for-the-badge&logo=react&logoColor=white)
- ![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
- ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
- ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

It was a challenging but rewarding week. 💪❤️
