# Pokédex

A React app that lets you explore every Pokémon using the pokeAPI. (https://pokeapi.co).

---

## Quick Start

```bash
npm install
npm start
```

Opens at **http://localhost:3000**

---

## Features

- **Random Pokémon** — roll a random pick with one click
- **Search** — find any Pokémon by name or Pokédex number
- **Evolution chain** — browse all evolutions, click to navigate
- **Favorites** — save your favorites (persisted to localStorage)
- **Shiny toggle** — view the shiny sprite
- **Type filter** — filter random rolls by type
- **Prev/Next navigation** — step through the Pokédex
- **Jest tests** — 30+ tests covering components and API utils

---

## Running Tests

```bash
# Interactive watch mode
npm test

# Full coverage report
npm run test:coverage
```

---

## Project Structure

```
pokedex/
├── public/
│   └── index.html                    # HTML shell
├── src/
│   ├── components/
│   │   ├── TypeBadge.js              # Type pill badge
│   │   ├── StatBar.js                # Animated stat bar
│   │   ├── EvolutionChain.js         # Evolution navigator
│   │   ├── SearchBar.js              # Search input + button
│   │   ├── FavoritesPanel.js         # Saved favorites grid
│   │   └── PokemonCard.js            # Main Pokémon display card
│   ├── __tests__/
│   │   ├── api.test.js               # API utility unit tests
│   │   ├── components.test.js        # TypeBadge + StatBar tests
│   │   ├── SearchBar.test.js         # SearchBar interaction tests
│   │   └── App.test.js               # Integration tests (mocked fetch)
│   ├── api.js                        # PokeAPI fetch helpers
│   ├── App.js                        # Main app component
│   ├── App.css                       # Design system styles
│   ├── index.js                      # React entry point
│   ├── index.css                     # Global reset + CSS variables
│   └── setupTests.js                 # Jest + Testing Library setup
├── .gitignore
└── package.json
```

---

## API

This app uses the free [PokeAPI](https://pokeapi.co) — **no API key or sign-up required**.

Endpoints used:
- `GET /pokemon/{name}` — stats, types, sprites, abilities
- `GET /pokemon-species/{name}` — flavor text, genus, evolution chain URL
- `GET /evolution-chain/{id}` — full evolution tree

---

## Deployment

```bash
npm run build
```

Deploy the `build/` folder to Netlify, Vercel, or GitHub Pages (free).

---

## Tech Stack

- **React 18** — UI & state
- **PokeAPI** — Pokémon data (free, no key)
- **Jest + React Testing Library** — tests
- **CSS custom properties** — full design system, no UI library

---

## Milestone Checklist

- [x] **Milestone 1** — Hello World / project running
- [x] **Milestone 2** — fetch from PokeAPI, display JSON data
- [x] **Milestone 3** — full UI + Jest tests
- [x] **Milestone 4** — polished CSS (custom fonts, animations, type colors)
