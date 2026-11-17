# Zoomer

A small search site. The page is in `public/`, and `netlify/functions/search.mts` calls the search service.

## Setup
1. Push this folder to a GitHub repo.
2. In Netlify: Add new project > Import from Git > pick the repo. No build command needed.
3. Nothing is needed for a first version: with no settings, Zoomer searches Marginalia (free, no signup). To use something else, add ONE of these under Site configuration > Environment variables:
   - `SERPER_API_KEY` (Google results via serper.dev)
   - `BRAVE_API_KEY` (Brave's own index)
   - `SEARXNG_URL` (address of your own SearXNG server, with JSON output enabled)
   - `MARGINALIA_API_KEY` (optional: your own Marginalia key, avoids the shared rate limit)
4. Redeploy if you added a setting. Open the site and search.
