# 🐱 Floppy Moo


This is a dark, moody browser-based Flappy Bird-style game starring **Moo** — a grey cat navigating a midnight world of pipes, seafood, and power-ups.

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
| `Tap upper/lower half` | Move up/down *(Wings mode, mobile)* |
| `Escape` / `P` | Pause / resume |

---

## Power-Ups

| Item | Effect | Spawn chance |
|---|---|---|
| ❤️ Heart | Extra life buffer (up to 5) — absorbs one pipe hit | ~35% |
| 🛡️ Shield | 10s immunity to pipe damage. Picking up a second shield while active adds 3s instead of resetting to 10s | ~31% |
| 🧲 Magnet | 10s attraction — all collectibles on screen float toward Moo | ~15% |
| 🔍 Magnify | 15s enlargement — all catchable items triple in size; guarantees 2 bonus collectibles spawn immediately | ~15% |
| 🪽 Wings | 10s free flight — use ↑/↓ to move freely, immune to pipes | ~4% |

*Spawn chances are per power-up roll (30% chance per pipe). Crab slow-motion only appears after 500 points.*

---

## Seafood

Seafood items spawn randomly between pipes (20% chance per pipe) and grant special bonuses:

| Item | Effect |
|---|---|
| 🐟 Fish | 2× score multiplier for 15 seconds |
| 🦐 Shrimp | +1 heart (extra life) |
| 🦀 Crab | Bullet time — pipes slow to 30% speed while Moo stays fast *(unlocks at 500 pts)* |
| 🦞 Lobster | Instant +5 points |

---

## Features

- **Difficulty scaling** — speed increases by 8% every 10 points; pipe spacing increases after 1000 points
- **Narrowing gaps** — pipe gap shrinks gradually as score climbs, flooring at a minimum to stay fair
- **Drifting pipes** — 40% of pipes slowly drift up or down, bouncing when they hit the boundary
- **Oscillating pipes** — 28% of pipes pulse their gap size open and closed (marked with a subtle blue tint on the caps)
- **Double pipes** — occasionally two pipes appear back-to-back in quick succession
- **High/low alternation** — gap positions bias to alternate between high and low, creating a rhythm
- **Wide → narrow rhythm** — a generous gap is sometimes immediately followed by a tighter one
- **Breakable pipes** — if Moo has a shield when hitting a pipe, the pipe shatters instead of bouncing him back
- **Edge collectibles** — some power-ups spawn right at the rim of the gap, requiring precision to grab
- **Near-miss sparks** — passing within ~18px of a pipe without hitting triggers golden sparks and a "close!" popup
- **Pipe color shift** — pipes gradually change from green to blue-purple as score climbs
- **Magnet** — attracts all on-screen collectibles toward Moo for 10 seconds
- **Magnify** — triples the size of all catchable items for 15 seconds; spawns 2 bonus collectibles immediately
- **Shield stacking** — catching a second shield while shielded adds 3s instead of resetting the timer
- **Slow-mo gating** — crab (bullet time) only starts appearing at 500+ points
- **Frame-rate independent** — delta-time loop ensures identical gameplay speed on all displays (60Hz, 120Hz, mobile, etc.)
- **Fullscreen mode** — scales to fit any screen via the ⛶ button
- **Pause / resume** — works on both desktop (P / Escape) and mobile (pause button)
- **Mobile wings** — tap upper/lower half of the screen to move Moo up/down during Wings mode
- **Procedural audio** — all sound effects generated via the Web Audio API (no audio files)
- **Hit invincibility** — brief blink + bounce when taking damage
- **Persistent best score** — tracked for the session

---

## Running the Game

Just open `index.html` in any modern browser. No server required.

```bash
open index.html
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
