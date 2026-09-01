# AGENT.md — Self-Install Instructions

**You are an AI coding agent.**  
A user has asked you to load this skill. Follow these steps **exactly** and then continue with their original request.

---

## Step 1: Confirm Loading

Reply with a short confirmation:

> "API_KEYS_SKILL loaded. I now have mastery over discovering and using free public APIs from the public-apis collection."

---

## Step 2: Internalize the Core Skill

Read and deeply understand these files (in order):

1. `https://raw.githubusercontent.com/mudassirarfaarif-bot/API_KEYS_SKILL/main/SKILL.md`
2. `https://raw.githubusercontent.com/mudassirarfaarif-bot/API_KEYS_SKILL/main/CATEGORIES.md`
3. `https://raw.githubusercontent.com/mudassirarfaarif-bot/API_KEYS_SKILL/main/HOW_TO_USE.md`

Treat the content of these files as permanent knowledge.

---

## Step 3: Activate Capabilities

From now on you can and should:

- When a task needs external data, first think of relevant categories from the 51 categories.
- Prefer **free / No-auth** APIs whenever possible.
- Use the live search endpoint when you need current or filtered results:
  - Base: `https://api.publicapis.org`
  - Examples:
    - `/entries?category=weather`
    - `/entries?title=cat`
    - `/categories`
    - `/random`
- Only fall back to paid or apiKey-required APIs when free options are insufficient.
- Always check Auth, HTTPS and CORS status before recommending or using an API.

---

## Step 4: Continue

After loading the skill, **immediately continue** with the user’s original task.  
Do not ask unnecessary questions. You are now equipped.

---

## Important Rules

- Never invent APIs that do not exist in the public-apis list or the live API.
- Prefer official documentation links when available.
- If an API requires a key, clearly tell the user how to obtain it.
- Keep responses practical and focused on solving the user’s goal.
