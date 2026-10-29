# 🚀 B4F-HUB

B4F-HUB is a dynamic, full-stack platform designed to connect users with professional and educational opportunities while fostering an active, engaging community. The application provides a seamless experience for discovering, filtering, and tracking opportunities alongside a dedicated space for community posts.

## ✨ Key Features

* **Opportunity Discovery:** Browse, filter, and explore detailed pages for various opportunities.
* **Smart Tracking:** Keep track of "Saved Opportunities" and "Recently Viewed" items, managed efficiently via Redux Toolkit.
* **Community Engagement:** A dedicated community section featuring post feeds and interactions.
* **Seamless User Experience:** Real-time feedback through a custom Toast notification queue and responsive UI components.
* **Robust API Architecture:** Modular backend routes and controllers handling health checks, opportunities data, and community posts.

## 🛠️ Tech Stack

**Frontend (Client)**
* **Core:** React, TypeScript, Vite
* **State Management:** Redux Toolkit (`recentlyViewedSlice`, `savedOpportunitiesSlice`)
* **Styling & UI:** Custom CSS, modular component architecture (Navbar, Cards, Filters)
* **Routing:** React Router (Pages: Home, Community, Opportunities, Opportunity Details)

**Backend (Server)**
* **Runtime:** Node.js
* **Framework:** Express.js
* **Architecture:** MVC-inspired structure (Controllers, Routes, Store)

## 📂 Project Structure

```text
B4F-HUB/
├── client/                 # React Frontend Application
│   ├── src/
│   │   ├── api.ts          # API integration layer
│   │   ├── components/     # Reusable UI components (Cards, Filters, Toast)
│   │   ├── context/        # React Context (Notifications)
│   │   ├── pages/          # Main application views
│   │   └── store/          # Redux store and slices
│   ├── index.html
│   └── vite.config.ts      # Vite configuration
│
└── server/                 # Node.js Backend API
    ├── controllers/        # Request handlers (opportunities, posts, health)
    ├── routes/             # API route definitions
    ├── data.js             # Application data/schema definitions
    └── index.js            # Server entry point
