# 🐱 FloppyMoo

A dark, moody browser-based Flappy Bird-style game starring **Moo** — a grey cat navigating a midnight world of pipes, seafood, and power-ups.

Built as a single self-contained HTML file. No dependencies, no build step.

---

## Gameplay

Guide Moo through gaps between pipes by tapping, clicking, or pressing Space/↑. The world speeds up as your score climbs. Collect power-ups and seafood along the way to survive longer and rack up points.

---

## Controls

| Input | Action |
|---|---|
| `Space` / `↑` | Flap / start game / restart |
| `↓` | Move down *(Wings mode only)* |
| `Click` / `Tap` | Flap / start game / restart |
| `Escape` / `P` | Pause / resume |

---

## Power-Ups

| Item | Effect |
|---|---|
| ❤️ Heart | Extra life buffer (up to 5) — absorbs one pipe hit |
| 🛡️ Shield | 10s immunity to pipe damage (no hearts lost on hit) |
| 🪽 Wings | 10s free flight — use ↑/↓ to move freely, immune to pipes |

---

## Seafood

Seafood items spawn randomly between pipes and grant special bonuses:

| Item | Effect |
|---|---|
| 🐟 Fish | 2× score multiplier for 15 seconds |
| 🦐 Shrimp | +1 heart (extra life) |
| 🦀 Crab | Bullet time — pipes slow to 30% speed while Moo stays fast |
| 🦞 Lobster | Instant +5 points |

---

## Features

- **Difficulty scaling** — speed increases by 8% every 10 points
- **Fullscreen mode** — scales to fit any screen via the ⛶ button
- **Pause / resume** — mid-game pause with visual overlay
- **Procedural audio** — all sound effects generated via the Web Audio API (no audio files)
- **Hit invincibility** — brief blink + bounce when taking damage
- **Persistent best score** — tracked for the session

---

## Running the Game

Just open `FloppyMoo.html` in any modern browser. No server required.

```bash
open FloppyMoo.html
```

Or drag the file into a browser window.

---

## Built With

- Vanilla JavaScript
- HTML5 Canvas
- Web Audio API

---

## About

FloppyMoo is a side project built for fun. Moo is a grey cat who deserves to fly.
