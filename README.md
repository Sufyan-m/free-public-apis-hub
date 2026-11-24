<div align="center">

# 🌐 Free Public APIs Hub
### Curated & Tested Collection of 48+ Free APIs for Python Developers, Bots & Automation

[![Python](https://shields.io)](https://python.org)
[![APIs](https://shields.io)](https://github.com)
[![No API Key](https://shields.io)](https://github.com)
[![PRs Welcome](https://shields.io)](https://github.com)

**Stop wasting hours hunting for dead endpoints.**  
Every API listed below is active, beginner-friendly, and ready to use with Python's `requests` library.

[Quick Start](#-how-to-use-quick-start) • [Anime](#-1-anime--manga-apis) • [Gaming](#-2-gaming--esports-apis) • [Crypto](#-3-crypto--finance-apis) • [Weather](#-4-weather--environment-apis) • [AI](#-5-ai--nlp-apis) • [Dev Tools](#-6-developer--utility-tools)

</div>

---

## 🚀 How to Use (Quick Start)

### 1. Install `requests`
```bash
pip install requests
```

### 2. Fetch Live Data in 5 Lines of Python
All `No Key` APIs work instantly without signup or authentication headers:

```python
import requests

# Example: Fetch live Anime rating & episode count
url = "https://jikan.moe on titan&limit=1"
response = requests.get(url, timeout=10).json()

anime = response["data"][0]
print(f"Title: {anime['title']} | Score: {anime['score']}/10 | Episodes: {anime['episodes']}")
```

### 3. Using `Free Key` APIs Safely
For APIs marked **`Free Key`**, never hardcode your key inside public GitHub files. Store it in a `.env` file:
```python
import os, requests

API_KEY = os.getenv("GEMINI_API_KEY")
```

---

## 📑 Table of Contents
- [🎌 1. Anime & Manga APIs](#-1-anime--manga-apis)
- [🎮 2. Gaming & Esports APIs](#-2-gaming--esports-apis)
- [💰 3. Crypto & Finance APIs](#-3-crypto--finance-apis)
- [🌤️ 4. Weather & Environment APIs](#-4-weather--environment-apis)
- [🤖 5. AI & NLP APIs](#-5-ai--nlp-apis)
- [🛠️ 6. Developer & Utility Tools](#-6-developer--utility-tools)
- [📚 7. Knowledge, Space & Media APIs](#-7-knowledge-space--media-apis)
- [🎯 8. Fun, Trivia & Animals APIs](#-8-fun-trivia--animals-apis)

---

## 🎌 1. Anime & Manga APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 1 | **[Jikan API v4](https://jikan.moe)** | `No Key` | `https://jikan.moe` | MyAnimeList search bot, top-airing tracker |
| 2 | **[AniList GraphQL](https://gitbook.io)** | `No Key` | `https://anilist.co` | Trending anime schedules & manga stats |
| 3 | **[Trace.moe API](https://github.io)** | `No Key` | `https://trace.moe` | Reverse-search anime screenshots for episode info |
| 4 | **[Waifu.pics API](https://waifu.pics)** | `No Key` | `https://waifu.pics` | Random SFW anime reaction images for Discord bots |
| 5 | **[Nekos.best API](https://nekos.best)** | `No Key` | `https://nekos.best` | Anime roleplay GIFs with anime source names |
| 6 | **[Kitsu API](https://apiary.io)** | `No Key` | `https://kitsu.io[text]=bleach` | Anime & manga catalog search with streaming links |

---

## 🎮 2. Gaming & Esports APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 7 | **[FreeToGame API](https://freetogame.com)** | `No Key` | `https://freetogame.com` | Filter free-to-play PC/browser games by genre |
| 8 | **[CheapShark API](https://cheapshark.com)** | `No Key` | `https://cheapshark.com` | Steam & PC game price-drop alert bot |
| 9 | **[PokéAPI](https://pokeapi.co)** | `No Key` | `https://pokeapi.co` | Terminal Pokédex or Discord battle mini-game |
| 10 | **[OpenDota API](https://opendota.com)** | `No Key` | `https://opendota.com` | Live Dota 2 pro matches & hero win-rate tracker |
| 11 | **[Valorant-API](https://valorant-api.com)** | `No Key` | `https://valorant-api.comv1/agents` | Valorant agents, weapons, skins & map database |
| 12 | **[Chess.com PubAPI](https://chess.com)** | `No Key` | `https://chess.com` | Daily chess puzzle bot & player rating lookup |
| 13 | **[RAWG Games API](https://rawg.io)** | `Free Key` | `https://rawg.io` | 500,000+ games database with Metacritic scores |

---

## 💰 3. Crypto & Finance APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 14 | **[CoinGecko Public](https://coingecko.com)** | `No Key` | `https://coingecko.com` | Live crypto prices in USD & PKR |
| 15 | **[Binance Public API](https://binance.com)** | `No Key` | `https://binance.com` | Real-time second-by-second crypto ticker |
| 16 | **[Frankfurter FX](https://frankfurter.dev)** | `No Key` | `https://frankfurter.dev` | Live & historical foreign exchange rates |
| 17 | **[ExchangeRate-API](https://exchangerate-api.com)** | `No Key` | `https://er-api.com` | Live USD to PKR & 160+ world currencies |
| 18 | **[CoinPaprika API](https://coinpaprika.com)** | `No Key` | `https://coinpaprika.comv1/tickers/btc-bitcoin` | Crypto market caps & historical coin data |
| 19 | **[Alpha Vantage](https://alphavantage.co)** | `Free Key` | `https://alphavantage.co` | Stock market quotes & technical indicators |

---

## 🌤️ 4. Weather & Environment APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 20 | **[Open-Meteo Weather](https://open-meteo.com)** | `No Key` | `https://open-meteo.com` | Karachi & global hourly weather forecast |
| 21 | **[Open-Meteo Air Quality](https://open-meteo.com/air-quality-api)** | `No Key` | `https://open-meteo.com` | Live city air pollution (PM2.5 & AQI) alerts |
| 22 | **[Sunrise-Sunset API](https://sunrise-sunset.org)** | `No Key` | `https://sunrise-sunset.org` | Exact sunrise, sunset & twilight times |
| 23 | **[OpenWeatherMap](https://openweathermap.org)** | `Free Key` | `https://openweathermap.org` | City-name weather search & 5-day forecast |
| 24 | **[WeatherAPI.com](https://weatherapi.com)** | `Free Key` | `https://weatherapi.com` | Real-time weather, astronomy & alerts |

---

## 🤖 5. AI & NLP APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 25 | **[Google Gemini API](https://google.dev)** | `Free Key` | `https://googleapis.com` | Free-tier AI text generation & PDF chat bots |
| 26 | **[Groq Cloud API](https://groq.com)** | `Free Key` | `https://groq.com` | Ultra-fast free inference for Llama LLMs |
| 27 | **[Hugging Face API](https://huggingface.co)** | `Free Key` | `https://huggingface.co` | Run thousands of free open-source AI models |
| 28 | **[OpenRouter API](https://openrouter.ai)** | `Free Key` | `https://openrouter.ai` | Single API endpoint with `:free` LLM models |
| 29 | **[Datamuse Word API](https://datamuse.com)** | `No Key` | `https://datamuse.com` | Find synonyms, rhymes & autocomplete words |

---

## 🛠️ 6. Developer & Utility Tools

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
| 30 | **[GitHub REST API](https://github.com)** | `No Key` | `https://github.com` | Fetch user profiles, repo stars & commits |
| 31 | **[IPify API](https://ipify.org)** | `No Key` | `https://ipify.org` | Instantly detect your public IP address |
| 32 | **[goQR QR Code API](https://goqr.me)** | `No Key` | `https://qrserver.com` | Generate instant QR code PNGs from any URL |
| 33 | **[REST Countries API](https://restcountries.com)** | `No Key` | `https://restcountries.comv3.1/name/pakistan` | Country flags, populations, currencies & borders |
| 34 | **[QuickChart API](https://quickchart.io)** | `No Key` | `https://quickchart.io{type:'bar',data:{labels:['A','B'],datasets:[{data:[10,20]}]}}` | Generate PNG bar/line charts via URL for bots |
| 35 | **[HTTPBin Testing](https://httpbin.org)** | `No Key` | `https://httpbin.orgget` | Test Python headers, proxies & JSON payloads |
| 36 | **[JSONPlaceholder](https://typicode.com)** | `No Key` | `https://typicode.composts` | Fake REST API for testing GET/POST requests |

---

## 📚 7. Knowledge, Space & Media APIs

| # | API Name | Auth | Live Test Endpoint | Project Ideas |
| :-: | :--- | :-: | :--- | :--- |
Use code with caution.
| 37 | Wikipedia REST API | No Key | https://wikipedia.org | Fetch clean article summaries & thumbnails |
| 38 | Open Library API | No Key | https://openlibrary.org | Search millions of books, authors & ISBNs |
| 39 | SpaceX API v4 | No Key | https://spacexdata.com | Rocket launch schedules & booster landings |
| 40 | TVMaze API | No Key | https://tvmaze.com | TV show episodes, cast lists & air dates |
| 41 | TheMealDB API | No Key | https://themealdb.com | Search cooking recipes, ingredients & video links |
| 42 | NASA Open APIs | Free Key | https://nasa.gov | Astronomy Picture of the Day & Mars rover photos |
