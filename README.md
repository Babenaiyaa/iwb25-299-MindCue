# 🌟 MindCue - Weather & Mood Driven Activity Recommendation System
A real-world, Ballerina-powered intelligent experience app

MindCue is a location-aware web application that provides **personalized mood-based recommendations** for music, activities, motivation, and wellness.
It uses **Ballerina SwanLake** as the backend integration layer for handling weather lookups, API orchestration, and AI-powered suggestions and a **React** frontend for a smooth interactive user experience.

This project was built for the **“Innovate with Ballerina 2025”** competition and demonstrates how Ballerina can be used to integrate external APIs and create intelligent, real-world applications.

---

## 🚀 Features
- 🌦️ **Real-time Weather Integration** – fetches live weather data (temperature, humidity, condition) based on user’s city using OpenWeather API.
- 🤖 **AI-Powered Recommendations** – Suggests activities, mood boosters, motivational content, and playlists based on weather + user mood.
- 🎶 **Spotify Playlist Suggestion** – auto-generated playlists based on detected environment.
- 📍 **Location-Aware** – users can select or auto-detect their city.
- 🎨 **Interactive UI** – clean card-based layout optimized for simplicity.

---

## 🛠️ Tech Stack
- **Frontend:** React (JavaScript, CSS Animations, Cards-based UI)
- **Backend:** Ballerina Swan Lake, REST APIs, AI recommendation service (Gemini / custom logic)
- **APIs Used:** OpenWeather API, Spotify API
- **Other Tools:** Node.js, npm, GitHub, VS Code

---

## ⚙️ Installation & Setup

### Prerequisites
- [Node.js](https://nodejs.org/) (v16+ recommended)
- [Ballerina Swan Lake](https://ballerina.io/downloads/)
- [Git](https://git-scm.com/)

### Clone the Repository
```bash
git clone https://github.com/your-username/mindcue.git
cd mindcue
```

### Frontend set up
```bash
cd frontend
npm install
npm start
```

### Backend
```bash
cd backend
bal run
```

(to run separate modules) 
```bash
bal run recommendation.bal
bal run weather.bal
bal run news.bal
```

## Project Architecture
```bash
┌───────────────────────────┐
│        React Frontend      │
│  (User Interface Layer)    │
└──────────────┬────────────┘
               │ REST API Calls
               ▼
┌───────────────────────────┐
│     Ballerina Backend     │
│  ┌──────────────────────┐ │
│  │ Weather Module       │ │ → Calls OpenWeather API
│  ├──────────────────────┤ │
│  │ Recommendation Module│ │ → AI logic + mood mapping
│  ├──────────────────────┤ │
│  │ Music Module         │ │ → Generates playlists
│  └──────────────────────┘ │
└──────────────┬────────────┘
               │ External APIs
               ▼
      OpenWeather / Spotify / Gemini

```

## 🤝 Team
- Lead Developer: Babenaiyaa S
- Weather/AI Modules: Lisorthman V
- UI/UX & Content: Sinthujan S

---
### Thank You for Exploring MindCue
Feel free to open issues or send PRs!
If you use this project as a Ballerina learning reference, tag us. 🙌
