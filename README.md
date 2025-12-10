# -alx-project-0x14
# Movies App – API Documentation Review

## API Overview
The MoviesDatabase API provides access to a large collection of movie data including titles, release years, genres, posters, and other related metadata. It allows developers to fetch and filter movies based on different parameters such as year, genre, and pagination. This API is useful for building movie discovery and streaming-related applications.

## API Version
The MoviesDatabase API uses **version 1** as provided through RapidAPI.

## Available Endpoints
- **GET /titles**
  - Retrieves a list of movies.
  - Supports filtering by year, genre, and sorting options.
- **GET /titles/{id}**
  - Fetches detailed information about a specific movie using its ID.
- **GET /genres**
  - Retrieves the list of available movie genres.
- **GET /titles/search**
  - Allows searching movies by title keywords.

## Request and Response Format
### Request Example
```http
GET /titles?year=2023&sort=year.decr&limit=12&page=1
Headers:
x-rapidapi-key: YOUR_API_KEY
x-rapidapi-host: moviesdatabase.p.rapidapi.com
