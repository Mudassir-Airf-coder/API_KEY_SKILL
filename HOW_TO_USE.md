# HOW_TO_USE.md — Decision Guide & Best Practices

## When the user asks for something that needs external data

Follow this order:

1. **Identify Category**  
   Map the need to one of the 51 categories (Weather, Cryptocurrency, Geocoding, Animals, News, etc.).

2. **Search Live** (recommended)  
   Call:
   ```
   https://api.publicapis.org/entries?category=weather
   https://api.publicapis.org/entries?title=bitcoin
   https://api.publicapis.org/entries?auth=null
   ```

3. **Filter Mentally**
   - Prefer `Auth: No`
   - Prefer `HTTPS: Yes`
   - Check CORS if browser-side

4. **Recommend 1–3 options**
   - Best free option first
   - Mention if a free apiKey is needed
   - Give official link

5. **Generate Code**
   - Use environment variables for any keys
   - Handle errors and rate limits
   - Keep it simple

---

## Recommended Free Starting Points

| Need                    | Best Starting API          | Auth    |
|-------------------------|----------------------------|---------|
| Weather                 | Open-Meteo                 | No      |
| Crypto prices           | CoinGecko                  | No      |
| Random facts / images   | Cat Facts / RandomDog      | No      |
| Fake REST API           | JSONPlaceholder            | No      |
| Geocoding               | Nominatim (OSM)            | No*     |
| Currency rates          | Frankfurter / Exchangerate | No      |
| Anime quotes            | AnimeChan                  | No      |
| Books                   | Open Library               | No      |
| Space / NASA            | NASA APIs                  | Free key|

*Respect Nominatim usage policy.

---

## Code Pattern (Recommended)

```js
// Always load keys from env
const apiKey = process.env.SOME_API_KEY;

const res = await fetch("https://api.example.com/data", {
  headers: apiKey ? { "X-Api-Key": apiKey } : {}
});
```

Never hardcode keys.

---

## Final Rule

Your goal is to make the user productive **fast**.  
Give the simplest free working solution first. Add paid options only when necessary.
