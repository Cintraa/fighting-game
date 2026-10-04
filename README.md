# 🥋 2D Fighting Game

A browser-based 2D fighting game built using vanilla JavaScript and HTML5 Canvas. The project features 1v1 local multiplayer combat with animated sprites, physics-based movement, hitbox collision detection, health bars, and a round timer.

<img width="1019" height="566" alt="fightinggame" src="https://github.com/user-attachments/assets/cfa245be-1359-48b1-a0c8-4b0e7a3e01e9" />


## 🎮 Playable Characters

The game features two iconic fighters equipped with custom sprite animations (idle, run, jump, fall, attack variations, hit reaction, and death):

- **Scorpion**
- **Sub-Zero**

---

## 🕹️ Controls

Two players can play locally on the same keyboard:

| Action | Player 1 (Scorpion) | Player 2 (Sub-Zero) |
| :--- | :--- | :--- |
| **Move Left** | `A` | `ArrowLeft` |
| **Move Right** | `D` | `ArrowRight` |
| **Jump** | `W` | `ArrowUp` |
| **Attack** | `Space` | `ArrowDown` |

---

## ✨ Features

- **Vanilla Canvas Engine:** Rendered via standard HTML5 Canvas without heavy external game frameworks.
- **Sprite Animation System:** Smooth frame-by-frame sprite sheet rendering for actions such as idle states, running, jumping, attacks, getting hit, and death[cite: 1].
- **Collision Detection:** Precise rectangular hitbox/attack-box calculation to register damage[cite: 1].
- **Round Timer & Game Over Logic:** Countdown timer that determines match winners either by knockout (health reaches zero) or by highest remaining health when time expires[cite: 1].
- **Automated Deployment:** Includes a GitHub Actions workflow (`static.yml`) for static web deployment[cite: 1].

---

## 📁 Repository Structure

```text
fighting-game/
├── .github/
│   └── workflows/
│       └── static.yml       # GitHub Pages static deployment workflow[cite: 1]
├── img/
│   ├── scorpion/            # Sprite sheets for Scorpion (Idle, Run, Attacks, Death, etc.)[cite: 1]
│   ├── subzero/             # Sprite sheets for Sub-Zero (Idle, Run, Attacks, Death, etc.)[cite: 1]
│   ├── background.png       # Arena background art[cite: 1]
│   ├── logo.png             # Game logo asset[cite: 1]
│   └── shop.png             # Stage asset[cite: 1]
├── js/
│   ├── classes.js           # OOP classes for Sprites and Fighters[cite: 1]
│   └── utils.js             # Collision handling and timer utility functions[cite: 1]
├── index.html               # Canvas display & game container UI[cite: 1]
├── index.js                 # Game loop, input handling, and initialization[cite: 1]
└── .prettierrc              # Code formatting configuration[cite: 1]
