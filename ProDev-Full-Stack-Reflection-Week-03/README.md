# ProDev Full-Stack Weekly Reflection Journal

## 🐍Backend Reflection 

### 📌 Summary of What I Did
This week, I worked on backend concepts focusing on **Python decorators, context managers, and asynchronous programming** with SQLite.  

- Built decorators to **log queries**, **manage DB connections**, **handle transactions**, **retry on failure**, and **cache query results**.  
- Created **custom context managers** for opening/closing database connections and executing queries safely.  
- Implemented **asynchronous database queries** with `aiosqlite` and `asyncio.gather` to run multiple queries concurrently for better performance.  

👉 Overall, I learned how to write **cleaner, safer, and faster code** by letting Python handle database connections, transactions, and concurrency automatically.  

---

## 🛠️ Tech Stack & Tools
Here are the main tools and technologies I used:

- **Python** – Core language  
- **SQLite** – Database  
- **asyncio** – For asynchronous programming  
- **GitHub** – Version control & repo hosting  

---

# 🌟 Frontend (TypeScript) – Reflection  

This week, I explored **TypeScript fundamentals** through the ALX Frontend track.  
It was challenging but rewarding 💪✨  

## 📚 Tasks Completed  

### ✅ Task 1 – Basic Types  
- Learned about defining interfaces & typed objects.  
- Created a `Teacher` interface with optional fields.  

### ✅ Task 2 – Classes  
- Built `StudentClass` with methods:
  - `workOnHomework() → "Currently working"`  
  - `displayName() → firstName`  

### ✅ Task 3 – Advanced Types (Part 1)  
- Designed `DirectorInterface` & `TeacherInterface`.  
- Implemented `Director` and `Teacher` classes.  
- Wrote `createEmployee` function with type guards.  

### ✅ Task 4 – Advanced Types (Part 2)  
- Added `isDirector` type predicate & `executeWork` function.  
- Introduced string literal types with `Subjects` ("Math" | "History").  
- Created `teachClass()` function returning `"Teaching Math"` or `"Teaching History"`.  

### ✅ Task 5 – Ambient Declarations  
- Wrote `crud.d.ts` with type declarations.  
- Used `RowID` & `RowElement` types with CRUD functions.  
- Practiced triple-slash directives & type imports.  

### ✅ Task 6 – Namespaces & Declaration Merging  
- Created `Subjects` namespace with:  
  - `Teacher` interface  
  - `Subject` base class  
  - `Cpp`, `Java`, `React` subclasses  
- Explored declaration merging by extending `Teacher` interface with optional attributes.  

### ✅ Task 7 – Main Application  
- Instantiated `Cpp`, `Java`, and `React` subjects.  
- Created `cTeacher` with `experienceTeachingC = 10`.  
- Logged requirements & available teachers per subject.  

### ✅ Task 8 – Brand Convention & Nominal Typing  
- Defined `MajorCredits` & `MinorCredits` interfaces with unique branding.  
- Built `sumMajorCredits()` & `sumMinorCredits()` functions.  

---

## 🌈 Reflections  
- Learned the **power of strong typing** 🛡️.  
- Struggled with **namespaces vs ES modules**, but fixed it ✅.  
- Gained confidence in **TypeScript configs, classes, and type guards**.  
- Excited to apply these concepts in real projects 🚀.  



## ✨ Reflection
- I now understand how **decorators** can wrap functions to add powerful features.  
- I learned that **context managers** (`with` statements) help prevent mistakes by ensuring resources (like DB connections) are always cleaned up.  
- I practiced **asynchronous programming**, which lets multiple tasks run together, making my programs more efficient.  

This backend foundation feels solid, and I’m excited to connect it with the **frontend** part of my learning next!
