# 🎬 Movie Discovery Platform

A modern movie discovery web app for browsing, searching, and exploring movies through a clean, responsive interface powered by real-time movie data.

**Live Demo:** [View the application](https://movie-o4gz1dkur-preethamaditya6.vercel.app/)

---

## ✨ Overview

Discover movies, explore trending titles, and quickly find something worth watching.

The app integrates the **TMDB API** for movie data and pairs it with a responsive **React** interface built for fast, intuitive browsing. An **Appwrite-backed layer** tracks searches to power a live trending movies list.

---

## 🚀 Features

- 🎥 **Movie Discovery** — Browse a large collection of movies with rich posters and metadata.
- 🔥 **Trending Movies** — Surface popular titles through a dynamic trending algorithm driven by real search activity.
- 🔎 **Movie Search** — Instantly search for movies by title.
- 📱 **Responsive Design** — Optimized for desktop, tablet, and mobile screens.
- ⚡ **Fast & Interactive UI** — Smooth interactions with reusable React components.
- 🎨 **Modern Interface** — Dark, cinematic UI focused on visual discovery.
- 📊 **Usage Tracking** — Appwrite-backed data layer for tracking movie search activity and powering trending insights.
- 🧩 **Component-Based Architecture** — Modular React components designed for maintainability and reuse.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **React** | Component-based frontend development |
| **Tailwind CSS** | Responsive and utility-first styling |
| **Appwrite** | Backend services and data persistence |
| **TMDB API** | Movie data and metadata |
| **Vite** | Development server and build tooling |
| **React-use** | Utility hooks for React |

---

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
