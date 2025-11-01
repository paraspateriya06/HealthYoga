# 🧘‍♂️ HealthYoga – Problem-Focused Yoga Guidance Platform  

**Tech Stack:** React.js, Node.js, Express.js, Firebase, Tailwind CSS  
**Deployment:** Vercel (Frontend) | Firebase (Backend Services)  

## 🌿 Overview  

**HealthYoga** is a full-stack wellness web application designed to provide **personalized and problem-specific yoga guidance**.  
It bridges the gap between general yoga apps and individual health needs by helping users discover yoga poses and routines **tailored to their specific physical or mental issues** — like back pain, stress, or neck stiffness.  

Unlike traditional apps that offer generic yoga plans, HealthYoga uses user input and stored preferences to generate **focused, health-oriented recommendations**.  
The project aims to encourage preventive healthcare through accessible, guided yoga practice powered by modern web technologies.

---

## 💡 What This Project Does  

Here’s what happens behind the scenes when a user interacts with the app:

1. **User Registration & Authentication**  
   - Users can sign up or log in using **Email/Password** or **Google Sign-In**, handled securely via Firebase Authentication.  
   - Once authenticated, a unique user profile is created and stored in Firebase.

2. **Personalized Yoga Recommendation**  
   - On login, users select a health problem (e.g., back pain, stress, fatigue).  
   - The app fetches a curated yoga routine corresponding to that issue.  
   - Each routine includes details like pose name, duration, and step-by-step guidance.

3. **Real-Time Cloud Sync**  
   - Every action (saving favorites, progress, preferences) is stored in **Firebase Firestore**.  
   - This ensures instant syncing across all devices — users can start on one device and continue on another seamlessly.

4. **Dynamic and Responsive UI**  
   - The interface is built with **React.js and Tailwind CSS**, ensuring fluid navigation and clean design across screen sizes.  
   - Components load dynamically to reduce lag and improve performance.

5. **Performance and Deployment**  
   - Frontend deployed on **Vercel** with CI/CD integration for instant updates.  
   - Firebase backend handles authentication, hosting, and database services.  
   - Overall load time reduced by **35%** via optimized bundling and caching strategies.

---

## ✨ Key Features  

- 🧘‍♀️ **Personalized Yoga Plans** – Tailored routines for specific health issues.  
- 🔐 **Firebase Authentication** – Secure login via email or Google account.  
- ☁️ **Real-Time Data Sync** – Cloud-stored preferences accessible across devices.  
- ⚡ **Fast & Optimized Frontend** – 35% faster load time after optimization.  
- 📱 **Fully Responsive UI** – Consistent design from desktop to mobile.  
- 🚀 **CI/CD Integration** – Seamless deployment with Vercel pipeline.  
- 🧩 **Scalable Codebase** – Modular and component-driven architecture.  

---

## 🧰 Tech Stack Breakdown  

| Layer | Technology | Purpose |
|-------|-------------|----------|
| **Frontend** | React.js, Tailwind CSS | UI development, state management |
| **Backend** | Node.js, Express.js | API endpoints and routing logic |
| **Database** | Firebase Firestore | Real-time data storage and sync |
| **Authentication** | Firebase Auth | Secure user login and sessions |
| **Hosting** | Vercel (Frontend), Firebase (Backend) | Deployment and CI/CD |
| **Version Control** | Git & GitHub | Source management and collaboration |

---

## 🧩 Project Architecture  

HealthYoga/
│
├── client/ # React Frontend
│ ├── src/
│ │ ├── components/ # UI Components (Navbar, Cards, Loader, etc.)
│ │ ├── pages/ # Pages (Home, Login, Dashboard, YogaPlan)
│ │ ├── context/ # Auth and App Context Providers
│ │ ├── utils/ # Firebase configuration and helpers
│ │ └── App.jsx # Main Application File
│ └── package.json
│
├── server/ # Express Backend
│ ├── routes/ # API routes
│ ├── controllers/ # Core business logic
│ ├── models/ # Optional (for structured data)
│ └── server.js
│
├── .env # Environment Variables (Firebase Keys)
├── README.md
└── package.json
