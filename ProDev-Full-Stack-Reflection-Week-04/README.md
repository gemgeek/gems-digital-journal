# ProDev Weekly Full-Stack Reflection 🐍🖼🌸
This week for ProDev Backend was a deep dive into the backend development lifecycle, focused on designing and building a RESTful API from the ground up using Django and Django REST Framework. I also solidified my understanding of the data layer by creating models, serializers, and seeders.

---

## Project: Building a Django REST API for a Messaging App

I successfully built a functional API for a messaging service. The process covered every major stage of development, from initial setup to final testing.

### 1. Project Setup & Configuration
- **Tasks Completed:**
  - Initialized a new Django project (`messaging_app`) and a dedicated app (`chats`).
  - Set up and activated a Python virtual environment to manage dependencies.
  - Installed **Django** and **Django REST Framework (DRF)**.
  - Configured the project's `settings.py` to include the new apps and set up global API security rules for authentication and permissions.
- **Key Learning:** The importance of isolating project dependencies with a virtual environment. I also learned how to configure project-wide settings like default security rules in DRF, making the API secure from the start.

### 2. Data Modeling & Migrations
- **Tasks Completed:**
  - Designed the database schema and translated it into Django models.
  - Created a custom `User` model by extending Django's `AbstractUser` to add custom fields like `role` and `phone_number`.
  - Defined the `Conversation` and `Message` models.
  - Implemented relationships: a `ManyToManyField` for conversation participants and `ForeignKey` relationships for messages.
- **Key Learning:** I now understand how to model complex relationships in Django's ORM. A major lesson was learning to work with and satisfy a literal automated checker, which sometimes required explicitly defining fields that would normally be inherited. I also solidified my understanding of the two-step migration process (`makemigrations` and `migrate`).

### 3. API Serialization (The "Translator")
- **Tasks Completed:**
  - Created serializers for the `User`, `Conversation`, and `Message` models.
  - Implemented **nested serialization** to include a list of messages and participants directly within a conversation's API response.
  - Used advanced DRF features like `SerializerMethodField` and custom `validate` methods to meet specific requirements.
- **Key Learning:** I grasped the core concept of serializers as "translators" between complex Python objects and universal formats like JSON. Handling nested relationships was a key takeaway for building efficient and user-friendly APIs.

### 4. Views & URL Routing (The "Front Desk")
- **Tasks Completed:**
  - Implemented `ModelViewSet`s to handle all the standard API logic (GET, POST, DELETE, etc.) with minimal code.
  - Overrode the `get_queryset` method to ensure users can only see and interact with their own conversations and messages—a critical security feature.
  - Set up **nested URL routing** using `drf-nested-routers` to create logical API paths like `/api/conversations/<id>/messages/`.
  - Added default DRF `api-auth` URLs for the browsable API's login functionality.
- **Key Learning:** `ViewSets` and `Routers` are incredibly powerful for rapidly building conventional APIs. The most important lesson here was on data privacy and security by filtering querysets based on the logged-in user.

### 5. Running & Debugging
- **Tasks Completed:**
  - Successfully ran the application using `runserver`.
  - Created a `superuser` to test the API endpoints via DRF's browsable API.
  - Diagnosed and fixed several runtime errors, particularly `AttributeError` issues related to specific import patterns required by the checker.
- **Key Learning:** This was a practical lesson in the difference between static code analysis (what the checker does) and runtime execution. I learned how to read a Python traceback to find the exact source of an error and fix it.

---

## Milestone 2: Creating Models, Serializers, and Seeders

In addition to the messaging app, I also completed a milestone focused on the data layer.

- **Models & Serializers:** Similar to the project, this involved defining the data structure and the API "translators."
- **Seeders:** I learned about and implemented **seeders**. A seeder is a script used to populate a database with initial or fake data (e.g., creating 50 fake users for testing). This is an essential tool for development, as it allows you to test your API with realistic data without having to manually create every entry.
---

## ProDev Frontend
Frontend this week was a whirlwind of learning and building with modern frontend technologies! I progressed from scaffolding my first project to building dynamic, data-driven, and interactive user interfaces. It was challenging, but I'm proud of the three complete projects I set up.

## Project 1: The Airbnb UI Clone (Fundamentals) 🏠

This project was all about getting the fundamentals right. I learned how to set up a project from scratch and build the basic visual elements of a web page.

- **What I Did:**
  - 🚀 Scaffolded a new **Next.js** project with **TypeScript** and **Tailwind CSS**.
  - 📂 Set up basic file-based routing to create multiple pages (`/`, `/about`, `/landing`).
  - 🧱 Built static UI components like `Card`, `Pill`, and a dynamic `Button`.
  - 🔧 Made components reusable and dynamic by passing `props` and defining their types with TypeScript `interfaces`.
- **Key Learning:** My biggest takeaway was understanding how to break a UI down into small, reusable "LEGO bricks" (components) and control their appearance and content using props.

---
## Project 2: API Integration & Interactivity 🔄

Building on the first project, this assignment introduced me to working with external data and making the application interactive.

- **What I Did:**
  - 🌐 Fetched data from a real external API (JSONPlaceholder) using Next.js's `getStaticProps` for great performance.
  - 🗺️ Mapped over arrays of data to render dynamic lists of `PostCard` and `UserCard` components.
  - 💡 Managed component state for the first time using the `useState` React hook.
  - 팝업 Built interactive **modal forms** that appear when a user clicks a button, allowing for new post and user creation.
- **Key Learning:** This project taught me the core skill of fetching and displaying data from an API. I also got comfortable with managing state, which is key for creating interactive user experiences like pop-up forms.

---
## Project 3: Responsive Property Listing App (Layouts) 🖼️

This final project focused on professional project setup and creating a consistent, robust layout structure for a larger application.

- **What I Did:**
  - 🐙 Mastered different Git workflows for duplicating and setting up a new repository from a starter template.
  - 📦 Created a clean data structure using `constants` for sample data and `interfaces` for type definitions.
  - 🏗️ Built shared layout components (`Header`, `Footer`, `Layout`).
  - 🌍 Applied the `Layout` component globally using `pages/_app.tsx` to ensure a consistent look and feel across the entire application.
- **Key Learning:** I learned how to structure a larger application with a consistent layout. Using a main `Layout` component in `_app.tsx` is a powerful pattern for keeping the UI consistent and code maintainable.

---
## 🛠️ Tools & Technologies I Used This Week

* **Next.js** 🔼
* **React** ⚛️
* **TypeScript** 📘
* **Tailwind CSS** 💨
* **Git & GitHub** 🐙
