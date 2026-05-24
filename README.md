# Mobilya Mevzisi

A co-op tower defense and spatial puzzle game prototype built in HTML5 Canvas and JavaScript.

You defend an apartment by placing furniture on walls during the night. Each piece of furniture has a function — turret, economy, healing, buff, trap, or storage. During the day, enemies attack from windows, doors, and balconies, and your wall arrangement determines whether you survive.

**Furniture that doesn't touch the wall doesn't work during the day** — this constraint is the core design tension of the game.

---

## Play the Prototype

The game runs entirely in the browser. Open `mobilya_mevzisi.html` in any modern browser.

---

## Current Version: v0.9.8

**5562 lines, single HTML file, no dependencies.**

### Implemented Systems

- **Grid-based placement:** Drag-and-drop furniture onto walls, rotate with R, wall-contact detection
- **18 furniture types** across 7 categories: weapons, turrets (4 variants), economy, healing/buff, storage, support, traps
- **3+2 enemy types:** Standard, scout (fast), tank, breaker (wall damage), ram (heavy wall damage)
- **Elite bosses:** Elite (600 HP) and Elite-X (900 HP with ranged attacks)
- **Day/night cycle:** Night preparation phase (180s timer), daytime siege
- **Threat scoring system:** Each day has a threat value; defense setup value should match or exceed
- **47-ability progression system** across 5 tiers (white, green, blue, purple, gold)
- **Level/XP system** with quadratic curve scaling
- **Endless Mode** with procedural day generation after the initial 5 hardcoded days
- **Market system:** Random stock rotation, refresh option, price/shape trade-offs
- **Trap projection mechanic:** Outdoor projection preview, connection lines to triggers
- **Wall destruction:** Enemies can target and break walls
- **Wall entry points:** Windows, doors, balconies open progressively across days
- **Minimap, log panel, status panel**
- **Player movement, weapons, healing**
- **Buff systems:** Stove damage boost, music speed boost, wardrobe wall HP buff

---

## Design Goals

The game is designed around three core feelings:

1. **"It barely fit"** — the spatial puzzle of arranging furniture should always feel tight
2. **Threat vs setup tension** — every night carries a small anxiety; team coordination is required
3. **Comfort and threat together** — the home environment is visible, but danger comes from outside

---

## Tech Stack

- HTML5 Canvas
- Vanilla JavaScript
- No external libraries or frameworks
- Single-file architecture

---

## References

- **Loop Hero** — passive combat + placement loop
- **Rogue Tower** — placement puzzle in tower defense
- **Don't Starve Together** — day/night co-op rhythm
- **Tetris Effect** — shape-fitting tension

---

## Status

Active development. Unity port planned for mobile (touch input, Android build).
