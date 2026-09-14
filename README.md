<div align="center">

# 👾 Space Invaders — Arcade Pygame Project

**A polished, faithful remake of the 1978 arcade classic, built from scratch in Python and Pygame.**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pygame](https://img.shields.io/badge/Pygame-2.x-005d8a?style=for-the-badge)
![Genre](https://img.shields.io/badge/Genre-Arcade%20Shooter-ffd343?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Playable-brightgreen?style=for-the-badge)

</div>

<p align="center">
  <img src="images/space-invaders-screenshot.png" alt="Space Invaders gameplay — score, high score, alien swarm, bunkers and player ship" width="640"/>
  <br/>
  <em>Defend Earth. One pixel at a time.</em>
</p>

---

## 📸 Screenshots

| Gameplay |
|----------|
| <img src="images/space-invaders-screenshot.png" alt="Space Invaders in action — 55 alien invaders, 4 defensive bunkers, and your lone cannon" width="640"/> |

---

## ✨ Features

- 👾 **Full alien swarm** — 55 invaders across 3 distinct types in the classic 5 × 11 formation, marching and speeding up as their numbers dwindle
- 🛡️ **Destructible bunkers** — 4 defensive shields that absorb fire from both sides and erode pixel by pixel
- 🛸 **Mystery ship** — the red UFO flies across the top row for bonus points
- 🚀 **Smooth cannon controls** — glide along the bottom edge and blast back with rapid laser fire
- 🔊 **Retro sound design** — laser shots, explosion effects, and looping background music straight from the arcade era
- 🏆 **Persistent high score** — your best run is saved to `highscore.txt` between sessions
- 🎨 **Classic CRT aesthetic** — authentic sprites, arcade font (Bradley Gratis), and the iconic black-and-neon palette

---

## 🛠️ Tech Stack

| Component | Purpose |
|-----------|---------|
| [Python 3.10+](https://www.python.org/) | Core language |
| [Pygame](https://www.pygame.org/) | Windowing, rendering, input, and audio |

---

## 📁 Project Structure

```
Arcade-Pygame-Project/
├── pygame-space invaders/
│   ├── main.py        # Entry point — window, game loop, event handling
│   ├── game.py        # Game state, collision logic, scoring, level flow
│   ├── spaceship.py   # Player cannon (movement, firing, lives)
│   ├── alien.py       # Alien swarm behavior and movement patterns
│   ├── laser.py       # Projectile system (player + alien shots)
│   ├── obstacle.py    # Destructible bunker blocks
│   ├── Graphics/      # Sprites (aliens, cannon, UFO, bunker tiles)
│   ├── Sounds/        # Music and SFX (laser, explosion, music loop)
│   ├── Font/          # Arcade display font
│   └── highscore.txt  # Persistent best score
└── README.md
```

> ⚠️ **Note:** the game folder name contains a space — wrap paths in quotes when running commands (shown below).

---

## 🚀 Getting Started

### 1. Install the dependency

```bash
pip install pygame
```

### 2. Run the game

```bash
python "pygame-space invaders/main.py"
```

> Run the command from the **repository root** so the game can find its `Graphics/`, `Sounds/`, and `Font/` folders.

### 3. Play!

| Key | Action |
|-----|--------|
| ⬅️ ➡️ Arrow keys | Move the cannon |
| **Space** | Fire laser |
| **Esc** / close window | Quit |

---

## ⚙️ How It Works

- **Swarm intelligence** — the alien grid shifts direction when any invader touches the screen edge, and the march tempo scales with how few remain — exactly like the original's escalating tension.
- **Pixel-accurate bunkers** — each shield is a grid of individual blocks; every laser hit removes only the blocks it touches, so bunkers crumble realistically.
- **Fair alien fire** — invaders shoot semi-randomly from the frontmost row, keeping pressure on the player without feeling rigged.
- **Object-oriented design** — `Spaceship`, `Alien`, `Laser`, and `Obstacle` are separate classes, making the codebase easy to extend with new enemy types, power-ups, or levels.

---

## 🗺️ Roadmap / Ideas

- [ ] Multiple lives & game-over screen with restart
- [ ] Increasing difficulty per wave (faster swarm, more fire)
- [ ] Pause menu (P key)
- [ ] Joystick/gamepad support
- [ ] Score pop-up animations and screen shake on hits
- [ ] `.gitignore` for `__pycache__/`

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-idea`)
3. Commit your changes (`git commit -m "Add amazing idea"`)
4. Push to the branch (`git push origin feature/amazing-idea`)
5. Open a Pull Request

---

## 📜 License

No license specified yet. If you'd like others to use or contribute, consider adding an [MIT License](https://choosealicense.com/licenses/mit/).

> *Space Invaders® is a trademark of Taito. This is an educational, non-commercial fan remake.*

---

<div align="center">
  Made with 🐍 Python & 🎮 Pygame · Insert coin to continue
</div>

