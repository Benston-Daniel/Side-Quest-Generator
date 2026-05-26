# 🎮 Mumbai Side Quests
### *A pocket arcade for two people who refuse to be boring*

![Welcome Screen](screenshots/splash.png)

> Built for one specific trip. Two specific people. Maximum chaos.

---

## What is this?

This is a single-page web app that turns a Mumbai trip into an RPG.

You pick the places you're visiting that day — a beach, a café, a mall, wherever — and it spins up a random **Side Quest** you have to complete there. Things like freezing in the middle of a crowded footpath, ordering for each other blind, building a sandcastle and making strangers vote on it, or feeding each other the entire meal without breaking character.

It has a scoreboard, a quest log, a Rock Paper Scissors duel mini-game, and a very specific June 28th announcement on the splash screen.

---

## Why I built this

My friend Pooja lives in Mumbai. I don't. So when I finally visit, I wanted to make sure we actually *do things* instead of just ending up at the same café for 6 hours (not that there's anything wrong with that).

I wanted something that felt like a game, where the city is the level, the places we visit are the map, and the quests are the reason to be weird in public together.

So I built it. One HTML file. Drops straight into a browser. No apps, no accounts, no setup.

It ended up being more personal than I expected. There's a quest where you write each other letters to open in a year. One where you hold hands in silence for 10 minutes. One where you just... watch the full sunset with your phones away. Alongside the ones where you stage a fake breakup in a mall.

That balance felt right.

---

## Screenshots

| Splash Screen | Quest Engine | Scoreboard |
|---|---|---|
| ![Splash](screenshots/splash.png) | ![Quest](screenshots/quest.png) | ![Score](screenshots/score.png) |

| Places Builder | Quest Log | Mini Game |
|---|---|---|
| ![Places](screenshots/places.png) | ![Log](screenshots/log.png) | ![Duel](screenshots/duel.png) |

---

## Features

- **Trip Builder** — add the places you're visiting today, drag to reorder
- **Quest Engine** — spin for a random side quest matched to your locations
- **80+ quests** across 9 categories: Outdoor, Beach, Restaurant, Mall, Cinema, Flat, Explore, Personal, and Pure Chaos
- **Vibe Filter** — filter quests by mood: Chaotic / Wholesome / Brave / Childish / Intimate / Brainrot
- **Custom Quests** — add your own quests to the pool
- **Named Players** — Benston & Pooja, obviously (renameable)
- **Individual Points** — award points to whoever actually crushed the quest
- **Quest Log** — full history of everything you completed
- **Quick Duel** — Rock Paper Scissors mini-game with bonus points on the line
- **Persisted State** — scores and history survive page refreshes via localStorage
- **CRT Aesthetic** — scanlines, pixel font, neon everything, 90s arcade machine energy

---

## Try it

🕹️ **[Play it here →](https://[your-username].github.io/mumbai-side-quests)**

*(or just download `index.html` and open it in any browser — works fully offline)*

---

## Run it yourself

No install. No build step. No node_modules.

```bash
# Option 1: just open it
open index.html

# Option 2: local server if you prefer
npx serve .
```

---

## Deploy to GitHub Pages

1. Create a new GitHub repo
2. Upload `index.html` to the root
3. Go to **Settings → Pages → Deploy from branch: main, folder: / (root)**
4. Done — live at `https://[username].github.io/[repo-name]`

---

## Customize it

All the data lives inside the `<script>` tag in `index.html`:

- **Add places** → edit the `PLACES_DATA` array
- **Add quests** → edit the `SIDE_QUESTS` object (organized by category)
- **Change player names** → edit the default `players` state in the Alpine component, or rename in-app

---

## Built with

- [Alpine.js](https://alpinejs.dev/) — reactivity
- [Tailwind CSS](https://tailwindcss.com/) — layout
- [SortableJS](https://sortablejs.github.io/Sortable/) — drag and drop
- [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P) — the only font that matters

Zero backend. Zero database. One file.

---

*Made with a lot of enthusiasm and questionable judgment.*
