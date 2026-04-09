# 🎬 Movie Watchlist App

A modern full-stack web application that allows users to discover movies, manage a personal watchlist, and get AI-powered recommendations.

---

## 🚀 Project Overview

The **Movie Watchlist App** is designed to help users:

- 🔍 Search for movies  
- ➕ Add movies to a personal watchlist  
- ⭐ Rate and review movies  
- 🤖 Get AI-powered movie recommendations  
- 👤 Manage their own personalized dashboard  

This project is built using a **modern AI-powered stack** with a focus on scalability, simplicity, and user experience.

---

## 🧱 Tech Stack

### Frontend
- Bolt (AI-powered UI builder)
- HTML / CSS / JavaScript (generated & customized)

### Backend
- Supabase (Database + Authentication + APIs)

### APIs & Integrations
- OpenAI API (AI recommendations & insights)
- TMDB API (Movie search and metadata)

### Deployment
- Vercel / Netlify (Frontend)
- Supabase (Backend)

---

## ✨ Features

### 🔐 Authentication
- User signup & login (Supabase Auth)
- Secure session management

### 🎥 Movie Search
- Search movies using TMDB API
- Display movie posters, titles, and release years

### 📌 Watchlist Management
- Add/remove movies from watchlist
- Track movie status (watchlist / watched)

### ⭐ Rating & Reviews
- Rate movies (1–5 stars)
- Add personal reviews

### 🤖 AI-Powered Features
- Personalized movie recommendations
- AI-generated reviews
- Mood-based suggestions

---

## 🗂️ Database Schema (Supabase)

### `movies`
```sql
id (uuid)
title (text)
description (text)
release_year (int)
poster_url (text)
tmdb_id (text)
```

### `watchlist`
```sql
id (uuid)
user_id (uuid)
movie_id (uuid)
status (text)
rating (int)
review (text)
created_at (timestamp)
```

---

## 🔗 Architecture

```
Frontend (Bolt UI)
        ↓
Supabase (Auth + DB)
        ↓
External APIs:
   - TMDB API (Movies)
   - OpenAI API (AI Features)
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/movie-watchlist-app.git
cd movie-watchlist-app
```

---

### 2️⃣ Setup Supabase

- Create a project in Supabase  
- Enable Authentication (Email/Password)  
- Create tables using the schema above  
- Enable Row Level Security (RLS)

Example policy:
```sql
user_id = auth.uid()
```

---

### 3️⃣ Environment Variables

Create a `.env` file:

```env
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_key
OPENAI_API_KEY=your_openai_api_key
TMDB_API_KEY=your_tmdb_api_key
```

---

### 4️⃣ Run the App

If using local dev:

```bash
npm install
npm run dev
```

---

## 🤖 OpenAI Integration

### Example Use Cases

**Movie Recommendation Prompt**
```
Suggest 5 movies based on the user's watchlist and preferences.
```

**AI Review Generator**
```
Generate a short review for the movie: {movie_name}
```

---

## 📦 API Flow

```
User Action → Frontend → Supabase → External APIs → Response → UI
```

---

## 🚀 Deployment

- Deploy frontend to **Vercel** or **Netlify**
- Backend is managed by **Supabase**

---

## 💡 Future Enhancements

- 🎬 Trailer integration (YouTube API)
- 👥 Social sharing
- 📊 User analytics dashboard
- 🔔 Notifications
- 🧠 Advanced recommendation engine

---

## 💰 Monetization Ideas

- Freemium model
- Premium AI recommendations
- Affiliate links (OTT platforms)
- Ads integration

---

## ⚠️ Best Practices

- Use Row-Level Security (RLS)
- Secure API keys with environment variables
- Implement loading states & error handling
- Optimize API calls

---

## 🙌 Contribution

Contributions are welcome!

1. Fork the repository  
2. Create a new branch  
3. Make changes  
4. Submit a Pull Request  

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Raj Kumar**  
AI & Data Engineer | Full Stack Enthusiast  

---

## ⭐ Support

If you like this project:

👉 Star the repo  
👉 Share with others  
👉 Contribute improvements  
