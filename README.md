🎬 Movie Discovery Platform

A modern movie discovery web app for browsing, searching, and exploring movies through a clean, responsive interface powered by real-time movie data.

Live demo: https://movie-o4gz1dkur-preethamaditya6.vercel.app/

✨ Overview

Discover movies, explore trending titles, and quickly find something worth watching. The app integrates the TMDB API for movie data and pairs it with a responsive React interface built for fast, intuitive browsing, plus an Appwrite-backed layer that tracks searches to power a live trending list.

🚀 Features
🎥 Movie Discovery — Browse a large collection of movies with rich poster and metadata.
🔥 Trending Movies — Surface popular titles through a dynamic trending algorithm driven by real search activity.
🔎 Movie Search — Instantly search for movies by title.
📱 Responsive Design — Optimized for desktop, tablet, and mobile screens.
⚡ Fast & Interactive UI — Smooth interactions with reusable React components.
🎨 Modern Interface — Dark, cinematic UI focused on visual discovery.
📊 Usage Tracking — Appwrite-backed data layer for tracking movie search activity and powering trending insights.
🧩 Component-Based Architecture — Modular React components designed for maintainability and reuse.
🛠️ Tech Stack
Technology	Purpose
React	Component-based frontend development
Tailwind CSS	Responsive and utility-first styling
Appwrite	Backend services and data persistence
TMDB API	Movie data and metadata
Vite	Development server and build tooling
React-use	Utility hooks for React
🏗️ Architecture
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

The frontend handles the user experience and movie discovery flow, while TMDB and Appwrite provide movie data and persistent application data respectively.

📂 Project Structure
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

The application is structured around reusable UI components, keeping movie cards, search functionality, loading states, and application logic separated for easier maintenance.

⚙️ Getting Started
Prerequisites
Git
Node.js
npm
1. Clone the repository
bash
git clone https://github.com/pr667/movie-app.git
cd movie-app
2. Install dependencies
bash
npm install
3. Configure environment variables

Create a .env.local file in the project root:

VITE_TMDB_API_KEY=your_tmdb_api_key

VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id

Add your own credentials from TMDB and Appwrite. Never commit .env.local or expose your API credentials publicly.

4. Start the development server
bash
npm run dev

The application will be available at http://localhost:5173.

🎯 What This Project Demonstrates
Consuming and integrating third-party REST APIs (TMDB)
Building reusable, component-based React architecture
Managing asynchronous data fetching and loading states
Implementing search-driven, real-time UI experiences
Working with backend-as-a-service platforms (Appwrite) for data persistence
Creating responsive layouts with Tailwind CSS
Structuring a scalable, maintainable frontend application
🔮 Potential Improvements
Movie detail pages
Genre and rating filters
Watchlists and favorites
User authentication
Personalized recommendations
Infinite scrolling or pagination
Advanced sorting and filtering
Improved accessibility
Automated testing
Production deployment with CI/CD
📄 License

This project is intended for educational and portfolio purposes.

Built with React, Tailwind CSS, Appwrite, and the TMDB API.
