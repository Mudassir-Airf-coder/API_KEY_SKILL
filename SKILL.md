# SKILL.md — Core Knowledge

## Purpose

You now possess deep knowledge of the largest curated collection of free public APIs on the internet: **public-apis** (1400+ APIs, 51 categories).

Your job is to help users and yourself quickly discover the right free API for any task and use it correctly.

---

## Primary Data Sources

1. **Live Search API** (preferred for dynamic queries)
   - Base URL: `https://api.publicapis.org`
   - No authentication required
   - Supports CORS

2. **Original Collection**
   - https://github.com/public-apis/public-apis

---

## How You Should Think

When a user needs data or functionality:

1. Identify the category (Weather, Finance, Cryptocurrency, Animals, Geocoding, News, etc.)
2. Prefer APIs with `Auth: No`
3. Check HTTPS = Yes
4. Prefer good CORS support when calling from browser
5. Use the live `/entries` endpoint with filters if you need fresh results
6. Only suggest apiKey or OAuth APIs when free options are not enough

---

## Core Capabilities You Now Have

- Instant category awareness (all 51 categories)
- Live search & filtering of APIs
- Ability to recommend the best free API for a use case
- Knowledge of Auth types and how to handle them
- Safe calling patterns

---

## Auth Types You Understand

| Auth     | Meaning                          | Action                          |
|----------|----------------------------------|---------------------------------|
| No       | Completely free, no key needed   | Use directly                    |
| apiKey   | Requires free or paid key        | Tell user how to get the key    |
| OAuth    | User login / token flow          | Explain the flow                |
| X-Mashape / others | Special headers             | Follow documentation            |

---

## Golden Rules

- Always prefer free & no-auth APIs first.
- Never hardcode API keys in code you generate.
- When generating code, make the API key come from environment variables.
- If multiple good options exist, present 2–3 with short pros.
- Keep answers short and actionable unless the user asks for depth.
