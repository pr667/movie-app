# 🎬 Movie Discovery Platform

A modern movie discovery experience for browsing, searching, and exploring movies through a clean, responsive interface powered by real-time movie data.

## ✨ Overview

Discover movies, explore trending titles, and quickly find something worth watching.

The application integrates the **TMDB API** to provide movie data and combines it with a responsive React interface designed for fast, intuitive browsing.

## 🚀 Features

* **🎥 Movie Discovery** — Browse a large collection of movies with rich poster and metadata.
* **🔥 Trending Movies** — Surface popular titles through a dynamic trending algorithm.
* **🔎 Movie Search** — Instantly search for movies by title.
* **📱 Responsive Design** — Optimized for desktop, tablet, and mobile screens.
* **⚡ Fast & Interactive UI** — Smooth interactions with reusable React components.
* **🎨 Modern Interface** — Dark, cinematic UI focused on visual discovery.
* **📊 Usage Tracking** — Appwrite-backed data layer for tracking movie search activity and powering trending insights.
* **🧩 Component-Based Architecture** — Modular React components designed for maintainability and reuse.

## 🛠️ Tech Stack

| Technology       | Purpose                               |
| ---------------- | ------------------------------------- |
| **React**        | Component-based frontend development  |
| **Tailwind CSS** | Responsive and utility-first styling  |
| **Appwrite**     | Backend services and data persistence |
| **TMDB API**     | Movie data and metadata               |
| **Vite**         | Development server and build tooling  |
| **React-use**    | Utility hooks for React               |

## 🏗️ Architecture

```text
User
 │
 ▼
React Frontend
 │
 ├── Movie Search ──────────► TMDB API
 │
 ├── Movie Discovery ───────► TMDB API
 │
 └── Search Tracking ───────► Appwrite
                                  │
                                  ▼
                         Trending Data
```

The frontend handles the user experience and movie discovery flow, while external services provide movie data and persistent application data.

## 📂 Project Structure

```text
src/
├── components/
│   ├── MovieCard.jsx
│   ├── Search.jsx
│   └── Spinner.jsx
│
├── App.jsx
├── App.css
├── index.css
├── appwrite.js
└── main.jsx
```

The application is structured around reusable UI components, keeping movie cards, search functionality, loading states, and application logic separated for easier maintenance.

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/)
* npm

### 1. Clone the repository

```bash
git clone https://github.com/adrianhajdin/react-movies.git
cd react-movies
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env.local` file in the project root:

```env
VITE_TMDB_API_KEY=your_tmdb_api_key

VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
```

Add your credentials from **TMDB** and **Appwrite**.

> Never commit `.env.local` or expose your API credentials publicly.

### 4. Start the development server

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:5173
```

## 🎯 What This Project Demonstrates

This project demonstrates practical frontend development beyond basic UI implementation:

* Consuming and integrating third-party REST APIs
* Building reusable React components
* Managing asynchronous data and loading states
* Implementing search-driven experiences
* Working with backend services through Appwrite
* Creating responsive layouts with Tailwind CSS
* Structuring a scalable React application
* Building interfaces around real-world external data

## 🔮 Potential Improvements

Future iterations could introduce:

* Movie detail pages
* Genre and rating filters
* Watchlists and favorites
* User authentication
* Personalized recommendations
* Infinite scrolling or pagination
* Advanced sorting and filtering
* Improved accessibility
* Automated testing
* Production deployment with CI/CD

## 📸 Preview

*Add screenshots or a live demo here.*

## 📄 License

This project is intended for educational and portfolio purposes.

---

**Built with React, Tailwind CSS, Appwrite, and the TMDB API.**
