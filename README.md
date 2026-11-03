<<<<<<< HEAD
# 🎬 Netflix Movie & TV Show Discovery App

A simple, clean, and intuitive movie discovery application built with **Streamlit**, inspired by Netflix. Search through thousands of movies and TV shows, explore popular genres, view storylines and cast details, read authentic viewer reviews, and see visual catalog insights.

---

## ✨ Features

### 1. 🏠 Simple Home Page
- **Clean Netflix-Style Design**: Dark charcoal background with Netflix red accents (`#E50914`).
- **Prominent Search Bar**: Search for any movie or TV show immediately from the center of the homepage.
- **Key Catalog Numbers**: Total titles (8,807), Movies (6,131), and TV Shows (2,676).
- **Popular Genres**: One-click genre chips (Dramas, Comedies, Action, International, Documentaries, Family, Horror, Sci-Fi) that jump directly to matching titles.
- **Explore Netflix Content**: A showcase of featured titles with movie poster cards and details.

### 2. 🎬 Simple Search & Explore Experience
- **Search Anything**: Case-insensitive instant search by title, actor, director, or keyword.
- **Attractive Poster Cards**: Displays high-resolution posters (from TMDB) or clean Netflix-themed cards with title, year, type badge, rating, genre, and a short description.
- **Easy Filters**: A small, optional expandable filter section with Content Type, Release Year, Genre, Country, Content Rating, and a **Reset Filters** button.
- **Export Data**: Download your filtered search results as a CSV file with one click.

### 3. 🔍 Movie Details & Viewer Reviews
When you click **"View Details"** on any title:
- **Left Side**:
  - High-resolution movie/TV show poster.
  - Live TMDB Community Rating (e.g. ⭐ 8.4/10) with vote count.
  - Direct link to IMDb page if available.
- **Right Side**:
  - Full title, release year, runtime/seasons, content rating, and genre tags.
  - Tagline and storyline overview.
  - Director / Creators, Main Cast, and Country of origin.
  - Netflix availability info (date added, catalog ID).
- **Viewer Reviews Section**:
  - Genuine viewer reviews retrieved live from The Movie Database (TMDB).
  - Reviewer name, date, user rating, and review text.
  - Direct link to read the full review on TMDB.
  - Clearly displays *"No user reviews available for this title"* if none exist.
  - *No fake data or invented ratings are ever generated.*
- **Easy Back Navigation**: A clear **"← Back to Results"** button returns you to where you were.

### 4. 💡 Simple Insights Page
Six straightforward charts with plain-English explanations:
1. **Movies vs TV Shows**: Shows that movies make up ~70% of the catalog and TV shows make up ~30%.
2. **Most Popular Genres**: Visualizes the top genres (Dramas, International Movies, Comedies).
3. **Top Countries**: Shows the top production nations (United States, India, United Kingdom).
4. **Content Added Over Time**: Shows Netflix's rapid library growth between 2016 and 2019.
5. **Movie Durations**: Shows runtime distributions, with an average length around 100 minutes.
6. **TV Show Seasons**: Highlights that ~67% of shows have 1 season (miniseries and limited runs).

### 5. ℹ️ About Page
- Simple project overview and technical documentation.
- Step-by-step instructions on configuring your free TMDB API key.
- TMDB attribution disclaimer.

---

## 🔑 How to Configure the TMDB API Key (For Live Posters & Reviews)

The app works out of the box using your local dataset with clean styled poster placeholders. To enable live movie posters, backdrop imagery, and viewer reviews:

1. **Get a free TMDB API Key**:
   - Create a free account at [themoviedb.org/signup](https://www.themoviedb.org/signup).
   - Go to **Settings → API** ([themoviedb.org/settings/api](https://www.themoviedb.org/settings/api)).
   - Request an API Key (Developer / Personal use is free and instantaneous).

2. **Add the Key to `.streamlit/secrets.toml`**:
   - In this project directory, open `.streamlit/secrets.toml`.
   - Add your API key:
     ```toml
     TMDB_API_KEY = "your_actual_tmdb_api_key_here"
     ```

3. **Restart or reload the Streamlit app**:
   - The sidebar will show **"✓ TMDB API Connected"**, and live movie posters and reviews will appear automatically!

---

## 🚀 How to Run the Application

### 1. Activate your virtual environment:
```powershell
# On Windows (PowerShell):
.\.venv\Scripts\activate
```

### 2. Start the Streamlit application:
```powershell
streamlit run app.py
```

Open your browser to:
```
http://localhost:8501
```

---

## 📂 Project Structure

```
Netflix Movies and TV Shows Analysis/
├── app.py                     # Main simple & intuitive Streamlit movie discovery app
├── app_backup.py              # Preserved original backup file (unmodified)
├── requirements.txt           # Project dependencies (Streamlit, Plotly, Pandas, Requests)
├── README.md                  # Project documentation
├── .streamlit/
│   ├── secrets.toml           # Your private TMDB API key configuration
│   └── secrets.toml.example   # Example template for secrets
├── dataset/
│   └── netflix_titles.csv     # 8,807 Netflix records (preserved)
├── notebooks/
│   └── netflix_eda.ipynb      # Exploratory data analysis notebook (preserved)
└── visualizations/            # Static charts (preserved)
```

---

## 📄 Attribution
- Dataset: Netflix Movies and TV Shows dataset from Kaggle.
- This product uses the TMDB API but is not endorsed or certified by TMDB.
=======
