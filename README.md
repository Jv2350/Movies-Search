# Movie App

A small web application to search for movies and save favorites.

## Description

This app lets you search for movies and add them to a favorites list for quick access later. It uses a third-party movie API to fetch movie data.

## Features

- Search movies (title lookup)
- Add or remove movies from Favorites
- View a Favorites page

## Requirements

- Node.js 16+ or newer

## API

- This project uses The Movie Database (TMDb) API to fetch movie data (endpoints like `/movie/popular` and `/search/movie`).
- The app reads the API base URL and key from Vite environment variables: `VITE_BASE_URL` and `VITE_API_KEY`.

How to get keys:

- Create a free account at https://www.themoviedb.org and obtain an API key from your account settings.

Environment variables (create a `.env` file in the project root):

```env
VITE_API_KEY=your_tmdb_api_key_here
VITE_BASE_URL=https://api.themoviedb.org/3
```

After adding or changing `.env` values, restart the dev server.

## Install & Run

Install dependencies and start the dev server:

```bash
npm install
npm run dev
```

Open the app at `http://localhost:5173` (Vite default).

## Files of interest

- `index.html` — app title and root element
- `src/App.jsx` — main app component
- `src/components` — UI components (MovieCard, NavBar, etc.)

If you want the README to include contribution guidelines, tests, or a production build section, tell me which to add.
