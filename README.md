
<div align="center">

# 🌐 Free Public APIs Hub

### 50 APIs. Endless Possibilities. Zero Cost to Get Started.

**Discover, explore, and integrate free public APIs into your next Python project.**

A curated collection of 50 public APIs for Python developers, automation engineers, and Telegram/Discord bot builders.

<br/>

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![APIs](https://img.shields.io/badge/APIs-50-2ea44f?style=for-the-badge)](#-api-directory)
[![Keyless](https://img.shields.io/badge/Keyless-Ready-blue?style=for-the-badge)](#-authentication-guide)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge&logo=github)](#-contributing)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

<br/>

[Explore APIs](#-api-directory) ·
[Quick Start](#-quick-start) ·
[CLI Tester](#-interactive-python-cli-tester) ·
[Contributing](#-contributing)

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Quick Start](#-quick-start)
- [Interactive Python CLI Tester](#-interactive-python-cli-tester)
- [Python Example](#-python-example)
- [Repository Structure](#-repository-structure)
- [API Directory](#-api-directory)
  - [Anime & Manga](#-1-anime--manga)
  - [Gaming & Esports](#-2-gaming--esports)
  - [Crypto, Stocks & Currency](#-3-crypto-stocks--currency-exchange)
  - [Weather & Geolocation](#-4-weather-air-quality--geolocation)
  - [AI & Natural Language Processing](#-5-ai-llms--natural-language-processing)
  - [Developer Tools](#-6-developer-tools-qr-codes--testing)
  - [Movies, TV & Music](#-7-movies-tv-shows--music)
  - [Knowledge, Science & Space](#-8-knowledge-books-science--space)
  - [Food, Health & Fitness](#-9-food-health--fitness)
  - [Fun, Trivia & Animals](#-10-fun-trivia-quotes--animals)
- [Authentication Guide](#-authentication-guide)
- [Security](#-security-best-practices)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📖 About the Project

**Free Public APIs Hub** is an open-source collection of 50 public APIs covering multiple development categories.

Finding useful APIs is easy. Finding suitable APIs with understandable documentation, accessible endpoints, and practical use cases is where things become interesting.

This repository aims to make that process easier.

Whether you're learning Python, building automation scripts, developing Telegram bots, or experimenting with external services, this collection provides a starting point.

### 🎯 Project Goals

- Make API discovery easier for beginners.
- Encourage practical Python development.
- Provide examples of real-world HTTP requests.
- Introduce developers to REST and GraphQL.
- Encourage API-based automation projects.
- Build a community-maintained API directory.

## ✨ Features

| Feature | Description |
|---|---|
| 🌐 50 APIs | Ten development categories |
| 🔓 Keyless Access | Discover APIs that need no authentication |
| 🔑 Free-Key APIs | Explore services with free registration tiers |
| 🐍 Python Support | Examples using the Requests library |
| 🧪 Interactive CLI | Test selected APIs from your terminal |
| 💡 Project Ideas | Practical inspiration for every category |
| 📚 Documentation | Direct links to official documentation |
| 🤝 Open Source | Community contributions welcome |

---

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or newer
- Git
- pip
- Internet connection

### 1. Clone the repository

```bash
git clone https://github.com/Sufyan-m/free-public-apis-hub.git
```

### 2. Enter the project directory

```bash
cd free-public-apis-hub
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch the application

```bash
python main.py
```

You're ready to explore the interactive API tester.

---

## 💻 Interactive Python CLI Tester

The repository includes an interactive command-line application called `main.py`.

It demonstrates how Python can communicate with external APIs and retrieve useful information.

### Available Demonstrations

| Option | Feature | Description |
|---|---|---|
| 01 | 🎌 Anime Explorer | Retrieve anime information |
| 02 | 💰 Crypto in PKR | Explore cryptocurrency prices |
| 03 | 🌤️ Karachi Weather | Retrieve weather information |
| 04 | 🎮 Free PC Games | Discover free-to-play games |
| 05 | 😂 Developer Jokes | Retrieve programming jokes |
| 00 | 🚪 Exit | Close the application |

### Example CLI Interface

```text
========================================
          FREE PUBLIC APIs HUB
========================================

[1] Anime Explorer
[2] Crypto Prices (PKR)
[3] Karachi Weather
[4] Free PC Games
[5] Developer Jokes

[0] Exit

========================================
Select an option:
```

*Illustrative interface. Actual output depends on the implementation of `main.py`.*

---

## 🐍 Python Example

You don't need a complicated application to start working with APIs.

Here's a simple example using the Jikan API.

```python
import requests

url = "https://api.jikan.moe/v4/anime?q=naruto&limit=1"

response = requests.get(url, timeout=10)
response.raise_for_status()
data = response.json()
print(data["data"][0]["title"])
```

### Sample JSON Response

<details>
<summary>📦 Click to expand the example response</summary>

```json
{
  "data": [
    {
      "mal_id": 20,
      "title": "Naruto",
      "type": "TV",
      "episodes": 220,
      "status": "Finished Airing"
    }
  ]
}
```

</details>

*Simplified illustrative response showing selected fields.*

### Understanding the Code

1. Import the `requests` library.
2. Define the API endpoint.
3. Send an HTTP GET request.
4. Check the HTTP response.
5. Convert JSON into Python data.
6. Access the required information.

---

## 📂 Repository Structure

```text
free-public-apis-hub/
│
├── README.md
│
├── main.py
│
└── requirements.txt
```

### Dependencies

`requirements.txt`

```text
requests>=2.31.0
```

---

# 🌐 API Directory

**50 APIs across 10 categories.**

Authentication labels:

- 🟢 `No Key` : Public endpoint that does not require an API key for the example request.
- 🟡 `Free Key` : Requires registration or an API token. A free tier or free access option is available, subject to provider conditions.

**Endpoint notes:** GET endpoints are provided where possible. APIs that require POST requests, request bodies, or special headers are identified. Free access does not mean unlimited access. Providers can change availability, authentication, and rate limits.

---

## 🎌 1. Anime & Manga

Anime databases, manga discovery, characters, and anime information.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 01 | [Jikan API](https://docs.api.jikan.moe/) | 🟢 No Key | `https://api.jikan.moe/v4/anime?q=naruto&limit=1` | Anime Search Bot |
| 02 | [Kitsu API](https://kitsu.docs.apiary.io/) | 🟢 No Key | `https://kitsu.io/api/edge/anime?page%5Blimit%5D=5` | Anime Database |
| 03 | [AniList GraphQL](https://docs.anilist.co/) | 🟢 No Key | `https://graphql.anilist.co` | Anime Recommendation App |
| 04 | [MangaDex API](https://api.mangadex.org/docs/) | 🟢 No Key | `https://api.mangadex.org/manga?limit=5&includes%5B%5D=cover_art` | Manga Discovery Tool |
| 05 | [Nekos.best](https://nekos.best/) | 🟢 No Key | `https://nekos.best/api/v2/neko` | Anime Image Bot |

**Note:** AniList's GraphQL endpoint requires a POST request containing a GraphQL query. The URL alone is not a complete test request.

---

## 🎮 2. Gaming & Esports

Gaming databases, Pokémon information, game deals, and competitive gaming statistics.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 06 | [PokéAPI](https://pokeapi.co/docs/v2) | 🟢 No Key | `https://pokeapi.co/api/v2/pokemon/pikachu` | Pokémon Explorer |
| 07 | [FreeToGame](https://www.freetogame.com/api-doc) | 🟢 No Key | `https://www.freetogame.com/api/games` | Free PC Games Finder |
| 08 | [CheapShark](https://apidocs.cheapshark.com/) | 🟢 No Key | `https://www.cheapshark.com/api/1.0/deals?storeID=1` | Game Deals Tracker |
| 09 | [Chess.com Published Data](https://www.chess.com/news/view/published-data-api) | 🟢 No Key | `https://api.chess.com/pub/player/hikaru` | Chess Statistics Dashboard |
| 10 | [OpenDota](https://docs.opendota.com/) | 🟢 No Key | `https://api.opendota.com/api/heroStats` | Dota 2 Statistics App |

---

## 💰 3. Crypto, Stocks & Currency Exchange

Cryptocurrency market information, exchange rates, and financial data.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 11 | [Binance API](https://developers.binance.com/docs/binance-spot-api-docs) | 🟢 No Key | `https://api.binance.com/api/v3/ticker/price?symbol=BTCUSDT` | Crypto Price Tracker |
| 12 | [CoinPaprika](https://docs.coinpaprika.com/) | 🟢 No Key | `https://api.coinpaprika.com/v1/tickers/btc-bitcoin` | Crypto Market Dashboard |
| 13 | [Frankfurter](https://frankfurter.dev/) | 🟢 No Key | `https://api.frankfurter.dev/v2/rates?base=USD&quotes=PKR` | Currency Converter |
| 14 | [CoinGecko](https://docs.coingecko.com/) | 🟡 Free Key | `https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd` | Cryptocurrency Portfolio Viewer |
| 15 | [Alpha Vantage](https://www.alphavantage.co/documentation/) | 🟡 Free Key | `https://www.alphavantage.co/query?function=GLOBAL_QUOTE&symbol=IBM&apikey=YOUR_API_KEY` | Stock Market Dashboard |

*Financial data may be delayed or subject to free-tier restrictions. These APIs are for development and educational projects, not financial advice.*

---

## 🌤️ 4. Weather, Air Quality & Geolocation

Weather forecasts, environmental information, sunrise times, and geolocation.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 16 | [Open-Meteo Weather](https://open-meteo.com/en/docs) | 🟢 No Key | `https://api.open-meteo.com/v1/forecast?latitude=24.8607&longitude=67.0011&current=temperature_2m,relative_humidity_2m,wind_speed_10m` | Karachi Weather App |
| 17 | [Open-Meteo Air Quality](https://open-meteo.com/en/docs/air-quality-api) | 🟢 No Key | `https://air-quality-api.open-meteo.com/v1/air-quality?latitude=24.8607&longitude=67.0011&current=pm10,pm2_5,us_aqi` | Air Quality Dashboard |
| 18 | [Sunrise-Sunset](https://sunrise-sunset.org/api) | 🟢 No Key | `https://api.sunrise-sunset.org/json?lat=24.8607&lng=67.0011&formatted=0` | Sunrise & Sunset Tracker |
| 19 | [Open-Meteo Geocoding](https://open-meteo.com/en/docs/geocoding-api) | 🟢 No Key | `https://geocoding-api.open-meteo.com/v1/search?name=Karachi&count=5&language=en&format=json` | Location Search Tool |
| 20 | [IPify](https://www.ipify.org/) | 🟢 No Key | `https://api.ipify.org?format=json` | IP Information Utility |

---

## 🤖 5. AI, LLMs & Natural Language Processing

Language processing, AI model access, and text-based applications.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 21 | [Datamuse](https://www.datamuse.com/api/) | 🟢 No Key | `https://api.datamuse.com/words?rel_syn=happy` | Vocabulary Assistant |
| 22 | [Google Gemini](https://ai.google.dev/gemini-api/docs) | 🟡 Free Key | `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=YOUR_API_KEY` | AI Chatbot |
| 23 | [Groq Cloud](https://console.groq.com/docs/overview) | 🟡 Free Key | `https://api.groq.com/openai/v1/models` | AI Assistant |
| 24 | [Hugging Face Inference](https://huggingface.co/docs/api-inference/index) | 🟡 Free Key | `https://router.huggingface.co/v1/chat/completions` | NLP Application |
| 25 | [OpenRouter](https://openrouter.ai/docs/quickstart) | 🟡 Free Key | `https://openrouter.ai/api/v1/models` | Multi-Model AI Interface |

*AI providers require account credentials for authenticated inference. Free models, quotas, and availability vary. Some endpoints only list models without authentication, while generation requests require a key and a suitable request body.*

---

## 🛠️ 6. Developer Tools, QR Codes & Testing

Utilities for development, HTTP testing, data visualization, and application integration.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 26 | [GitHub REST API](https://docs.github.com/en/rest) | 🟢 No Key | `https://api.github.com/users/Sufyan-m` | GitHub Profile Analyzer |
| 27 | [JSONPlaceholder](https://jsonplaceholder.typicode.com/guide/) | 🟢 No Key | `https://jsonplaceholder.typicode.com/posts/1` | REST API Practice |
| 28 | [HTTPBin](https://httpbin.org/) | 🟢 No Key | `https://httpbin.org/get` | HTTP Request Tester |
| 29 | [QR Server API](https://goqr.me/api/) | 🟢 No Key | `https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=HelloWorld` | QR Code Generator |
| 30 | [REST Countries](https://restcountries.com/) | 🟢 No Key | `https://restcountries.com/v3.1/name/pakistan` | Country Information App |

---

## 🎬 7. Movies, TV Shows & Music

Explore movies, television series, music metadata, and entertainment information.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 31 | [TVMaze](https://www.tvmaze.com/api) | 🟢 No Key | `https://api.tvmaze.com/search/shows?q=breaking+bad` | TV Series Explorer |
| 32 | [MusicBrainz](https://musicbrainz.org/doc/MusicBrainz_API) | 🟢 No Key | `https://musicbrainz.org/ws/2/artist/?query=artist:radiohead&fmt=json` | Music Artist Explorer |
| 33 | [iTunes Search API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/) | 🟢 No Key | `https://itunes.apple.com/search?term=linkin+park&entity=song&limit=5` | Music Search App |
| 34 | [TheAudioDB](https://www.theaudiodb.com/api_guide.php) | 🟢 No Key | `https://www.theaudiodb.com/api/v1/json/123/search.php?s=coldplay` | Artist Information App |
| 35 | [OMDb API](https://www.omdbapi.com/) | 🟡 Free Key | `https://www.omdbapi.com/?t=Inception&apikey=YOUR_API_KEY` | Movie Information Dashboard |

*MusicBrainz requests should include an identifiable User-Agent and respect its rate limits. TheAudioDB's public test key may have restricted access. OMDb requires a registered key.*

---

## 📚 8. Knowledge, Books, Science & Space

Discover encyclopedic information, books, space exploration, and scientific datasets.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 36 | [Wikipedia REST API](https://en.wikipedia.org/api/rest_v1/) | 🟢 No Key | `https://en.wikipedia.org/api/rest_v1/page/summary/Python_(programming_language)` | Wikipedia Search Tool |
| 37 | [Open Library](https://openlibrary.org/developers/api) | 🟢 No Key | `https://openlibrary.org/search.json?q=python` | Book Finder |
| 38 | [SpaceX API](https://github.com/r-spacex/SpaceX-API) | 🟢 No Key | `https://api.spacexdata.com/v4/launches/latest` | Space Mission Tracker |
| 39 | [GBIF API](https://techdocs.gbif.org/en/openapi/) | 🟢 No Key | `https://api.gbif.org/v1/species/match?name=Panthera+tigris` | Biodiversity Explorer |
| 40 | [NASA Open APIs](https://api.nasa.gov/) | 🟡 Free Key | `https://api.nasa.gov/planetary/apod?api_key=DEMO_KEY` | Astronomy Explorer |

*NASA's DEMO_KEY is intended for limited demonstration use. Obtain your own key for regular development.*

---

## 🍔 9. Food, Health & Fitness

Food databases, recipes, nutritional information, and exercise-related datasets.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 41 | [TheMealDB](https://www.themealdb.com/api.php) | 🟢 No Key | `https://www.themealdb.com/api/json/v1/1/search.php?s=Arrabiata` | Recipe Finder |
| 42 | [Open Food Facts](https://openfoodfacts.github.io/openfoodfacts-server/api/) | 🟢 No Key | `https://world.openfoodfacts.org/api/v2/product/737628064502.json` | Food Product Explorer |
| 43 | [Fruityvice](https://www.fruityvice.com/) | 🟢 No Key | `https://www.fruityvice.com/api/fruit/all` | Fruit Information App |
| 44 | [USDA FoodData Central](https://fdc.nal.usda.gov/api-guide.html) | 🟡 Free Key | `https://api.nal.usda.gov/fdc/v1/foods/search?api_key=DEMO_KEY&query=apple` | Food Data Explorer |
| 45 | [wger Workout Manager](https://wger.de/en/software/api) | 🟢 No Key* | `https://wger.de/api/v2/exerciseinfo/?language=2&limit=5` | Exercise Information App |

*Check the provider's current API authentication and access requirements before relying on anonymous access. Food and exercise data are informational, not personalized medical or fitness advice.*

---

## 🎯 10. Fun, Trivia, Quotes & Animals

Random trivia, jokes, advice, and animal-related information.

| # | API Name | Auth | Working Test Endpoint | Best Project Use Case |
|---|---|---|---|---|
| 46 | [Open Trivia DB](https://opentdb.com/api_config.php) | 🟢 No Key | `https://opentdb.com/api.php?amount=10&type=multiple` | Quiz Application |
| 47 | [JokeAPI](https://jokeapi.dev/) | 🟢 No Key | `https://v2.jokeapi.dev/joke/Programming?type=single` | Developer Joke Generator |
| 48 | [Advice Slip](https://api.adviceslip.com/) | 🟢 No Key | `https://api.adviceslip.com/advice` | Random Advice Bot |
| 49 | [Dog CEO API](https://dog.ceo/dog-api/) | 🟢 No Key | `https://dog.ceo/api/breeds/image/random` | Dog Image Generator |
| 50 | [TheCatAPI](https://thecatapi.com/) | 🟡 Free Key | `https://api.thecatapi.com/v1/images/search` | Cat Image Explorer |

---

## 🔐 Authentication Guide

Public APIs generally fall into two authentication categories.

### 🟢 No Key Required

These APIs allow public requests without registering for an API token.

Example:

```python
import requests

url = "https://pokeapi.co/api/v2/pokemon/pikachu"

response = requests.get(url, timeout=10)
response.raise_for_status()

pokemon = response.json()

print(pokemon["name"])
print(pokemon["height"])
```

### 🟡 Free API Key Required

Some services require registration before accessing their endpoints.

Example:

```python
import requests
import os

api_key = os.getenv("WEATHER_API_KEY")

url = "https://api.weatherapi.com/v1/current.json"

params = {
    "key": api_key,
    "q": "Karachi"
}

response = requests.get(url, params=params, timeout=10)
response.raise_for_status()

print(response.json())
```

### Important

A free API key does not necessarily mean unlimited requests.

Always check:

- Free-tier request limits.
- Authentication requirements.
- Usage restrictions.
- Commercial usage policies.
- Rate limits.
- Attribution requirements.

---

## 🔒 Security Best Practices

API keys are credentials. Treat them accordingly.

**Never commit private API keys to GitHub.**

Recommended practices:

1. Store credentials in environment variables.
2. Use `.env` for local development.
3. Add `.env` to `.gitignore`.
4. Never hardcode private credentials into public source files.
5. Rotate a key immediately if it is accidentally exposed.

### Example `.env`

```env
WEATHER_API_KEY=your_actual_api_key
GEMINI_API_KEY=your_actual_api_key
```

### Example `.gitignore`

```gitignore
.env
.venv/
venv/
__pycache__/
*.pyc
```

For larger applications, consider a dedicated secrets manager.

---

## 🧪 API Testing Recommendations

Before integrating an API into an application, examine its behavior.

| Test | What to Verify |
|---|---|
| HTTP Status | Does the request succeed? |
| JSON Parsing | Is the response valid JSON? |
| Authentication | Is a token required? |
| Rate Limits | What is the request allowance? |
| Timeout | Does the request finish within a reasonable time? |
| Error Handling | What happens when the service fails? |
| Documentation | Are the parameters and response fields documented? |

### Basic Error Handling

```python
import requests

url = "https://api.jikan.moe/v4/anime/1"

try:
    response = requests.get(url, timeout=10)
    response.raise_for_status()

    data = response.json()

    print(data)

except requests.exceptions.Timeout:
    print("The API request timed out.")

except requests.exceptions.HTTPError as error:
    print(f"HTTP error: {error}")

except requests.exceptions.RequestException as error:
    print(f"Request failed: {error}")

except ValueError:
    print("The API returned invalid JSON.")
```

---

## 💡 Project Ideas

Turn API experiments into practical development projects.

| Difficulty | Project | Suggested APIs |
|---|---|---|
| Beginner | Random Joke Generator | JokeAPI |
| Beginner | Anime Search Tool | Jikan |
| Beginner | Pokémon Information CLI | PokéAPI |
| Beginner | Currency Converter | Frankfurter |
| Beginner | Country Explorer | REST Countries |
| Beginner | Recipe Finder | TheMealDB |
| Intermediate | Karachi Weather Dashboard | Open-Meteo |
| Intermediate | Crypto Tracker in PKR | Binance + Frankfurter |
| Intermediate | Free PC Games Finder | FreeToGame |
| Intermediate | GitHub Profile Analyzer | GitHub REST |
| Intermediate | Movie Discovery Application | OMDb + TVMaze |
| Intermediate | Discord Information Bot | Multiple APIs |
| Advanced | Multi-API Automation System | Multiple APIs |
| Advanced | AI-Powered Assistant | Gemini / Groq |
| Advanced | Personal Data Dashboard | Multiple APIs |

**Recommended learning path:**

Start with one endpoint, understand its response, write a small Python function, and gradually combine multiple APIs.

The goal is not simply to send requests. It's to understand how external services become part of real applications.

---

## 🤝 Contributing

Contributions are welcome!

This project aims to grow into a useful, community-maintained resource for developers.

### What Can You Contribute?

- Add new public APIs.
- Report unavailable endpoints.
- Correct documentation links.
- Update authentication requirements.
- Improve Python examples.
- Suggest new project ideas.
- Improve `main.py`.
- Fix bugs and documentation issues.

### Contribution Workflow

**1. Fork the repository**

Click the Fork button on GitHub.

**2. Clone your fork**

```bash
git clone https://github.com/YOUR_USERNAME/free-public-apis-hub.git
```

**3. Enter the project**

```bash
cd free-public-apis-hub
```

**4. Create a feature branch**

```bash
git checkout -b feature/add-new-api
```

**5. Make your changes**

Follow the existing formatting and category structure.

**6. Commit your changes**

```bash
git add .
git commit -m "Add new public API"
```

**7. Push your branch**

```bash
git push origin feature/add-new-api
```

**8. Open a Pull Request**

Submit your changes to the original repository.

### API Submission Guidelines

Before submitting an API, ensure that:

- The service has official documentation.
- The endpoint uses HTTPS.
- The example request is valid.
- Authentication requirements are accurate.
- Free-tier restrictions are disclosed.
- The API is relevant to developers.
- The entry is not already listed.

Broken or discontinued APIs should be reported so the directory can be maintained.

---

## 📜 License

This project is licensed under the **MIT License**.

You are free to use, modify, distribute, and build upon this project according to the terms of the license.

See the [LICENSE](LICENSE) file for details.

---

## ⭐ Support the Project

If this repository helps you discover APIs or build something interesting:

- ⭐ Star the repository.
- 🍴 Fork it and experiment.
- 🐛 Report bugs.
- 💡 Suggest new APIs.
- 🤝 Contribute improvements.

Every contribution helps make this resource more useful.

---

<div align="center">

## 🌐 Free Public APIs Hub

**Discover APIs. Build Projects. Keep Learning.**

Created and maintained by **[@Sufyan-m](https://github.com/Sufyan-m)**

[GitHub Profile](https://github.com/Sufyan-m) · [Repository](https://github.com/Sufyan-m/free-public-apis-hub)

<sub>Built for developers, learners, and open-source enthusiasts.</sub>

**⭐ If you find this project useful, consider giving it a star!**

</div>
