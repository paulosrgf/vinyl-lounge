# Vinyl Lounge

> A minimalist static e-commerce catalog for vinyl record collectors — built entirely with Semantic HTML5 and Modern CSS3, no JavaScript frameworks required.

![HTML5](https://img.shields.io/badge/HTML5-Semantic-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Grid_%26_Flexbox-1572B6?style=flat-square&logo=css3&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-Alpine-009639?style=flat-square&logo=nginx&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## Overview

Vinyl Lounge is a front-end portfolio project centered around a **Noir Café Aesthetic** — warm sepia filters, rich brown tones, and soft dark contrast — designed to evoke the atmosphere of a late-afternoon music lounge.

The goal was to demonstrate advanced CSS layout techniques, responsive design patterns, and multi-state UI flows without relying on any JavaScript framework or build tool.

---

## Project Structure

```
vinyl-lounge/
│
├── index.html              # Homepage — Hero Banner & full catalog
├── collections.html        # Genres page with simulated search filtering
├── cart.html               # Active cart — table view with total pricing
├── cart-empty.html         # Empty cart state view
├── favicon.ico
│
├── style/
│   ├── style.css           # Global styles (resets, header, footer, hero)
│   └── style-pages.css     # Internal page layouts (cart, search, tables)
│
└── assets/
    └── images/
        └── covers/         # High-quality vinyl record artwork
```

---

## Features

**Glassmorphic Header** — Fixed top navigation with `backdrop-filter` blur for a premium layered effect.

**Editorial Section Layout** — Dark-inverted transition zones using italic numerals and deliberate vertical rhythm for structural contrast.

**Symmetric Product Grid** — Powered by `grid-template-columns: repeat(auto-fill, minmax(280px, 1fr))` and `grid-auto-rows: 1fr`, guaranteeing alignment regardless of badge or label variations.

**Simulated State Routing** — Anchor-based navigation (`href`) handles transitions between active cart, empty cart alerts, and filtered genre listings — no JavaScript required.

**Production-Safe Fallbacks** — All containers use explicit HEX values (`#231c18`, `#f7f5f0`) as fallbacks against external asset failures.

---

## Running Locally with Docker

The application is containerized using **Nginx (Alpine)** to serve static files with minimal overhead.

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Steps

**1. Clone the repository and navigate to the project root:**

```bash
cd VinylLounge
```

**2. Build and start the container:**

```bash
docker compose up -d --build
```

**3. Open in your browser:**

```
http://localhost:8080
```

**4. To stop the container:**

```bash
docker compose down
```

---

## Tech Stack

| Layer            | Technology                                             |
| ---------------- | ------------------------------------------------------ |
| Markup           | HTML5 (Semantic elements)                              |
| Styling          | CSS3 — Flexbox, Grid, Custom Properties, Media Queries |
| Server           | Nginx (Alpine)                                         |
| Containerization | Docker & Docker Compose                                |

---

## License

Open-source. Developed for academic and portfolio purposes.

_Spinning memories since 2026._
