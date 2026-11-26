# 🎈 Balloon Pop

A fun, single-file HTML balloon-popping game! Click on balloons to pop them and rack up points.

[**Play Now**](https://gadathagod.github.io/BaloonPop) · [**GitHub**](https://github.com/GadatheGod/BaloonPop)

---

## 🎮 How to Play

1. Open the game in your browser
2. Click **PLAY** on the start screen
3. **Click on balloons** to pop them and earn points
4. Chain quick pops for a **combo multiplier** 🔥
5. Keep popping — difficulty ramps up as you play!

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🎈 **4 Balloon Types** | Normal (1x), Gold (3x, sparkly), Tiny (fast), Big (2x) |
| 🔥 **Combo System** | Chain pops within 2s for a score multiplier |
| 🎵 **Sound Effects** | Pop sounds, level-up fanfare, combo ping |
| 💥 **Explosive Balloons** | Red balloons that chain-pop nearby balloons |
| ⚡ **Power-ups** | Slow-Mo, Double Points, and Freeze balloons |
| 🎆 **Pop Animations** | Expanding rings, particles, golden stars |
| 🌿 **Animated World** | Drifting clouds, swaying grass, sky gradient |
| 📈 **Endless** | No game over — just keep climbing your score |
| 🏆 **High Score** | Best score and best streak saved locally |
| 🎉 **Level-Up Confetti** | 60 confetti pieces burst on each level up |

---

## 🚀 Tech Stack

- **Single HTML file** — no build step, no dependencies
- **HTML5 Canvas** for rendering
- **Web Audio API** for sound (no external files)
- **localStorage** for high score persistence
- **Vanilla JavaScript** — no frameworks needed

---

## 🛠️ Run Locally

Just open the `index.html` file in any modern browser:

```bash
# Clone the repo
git clone https://github.com/GadatheGod/BaloonPop.git

# Open in browser
open index.html
```

Or deploy it anywhere:

```bash
# GitHub Pages (free)
# 1. Push to GitHub
# 2. Go to Settings > Pages > Source: main branch
# 3. Your game is live at https://<username>.github.io/BaloonPop
```

---

## 📐 Game Mechanics

### Scoring
| Balloon | Points | Rarity |
|---------|--------|--------|
| Normal 🔴 | 1x | Common |
| Gold ⭐ | 3x | Rare |
| Tiny ⚡ | 1x | Uncommon |
| Big 🟣 | 2x | Uncommon |

### Combo
- Pop balloons quickly (within 2 seconds) to build a combo
- Each balloon in the combo chain is multiplied by your current combo count
- Combo resets after 2 seconds of inactivity

### Levels
- Every **10 points** = Level Up
- Balloons get faster and more spawn per level
- Difficulty caps at a reasonable maximum

---

## 🎨 Customization

Want to tweak the game? Here are the key variables in the code:

```javascript
// Balloon type weights (higher = more common)
const BALLOON_TYPES = {
  normal: { weight: 60 },
  gold:   { weight: 10 },
  tiny:   { weight: 15 },
  big:    { weight: 15 },
};

// Level-up threshold
if (score % 10 === 0) { /* level up */ }

// Combo timeout (seconds)
comboTimer = 2;
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Credits

Built with ❤️ using vanilla HTML, CSS, and JavaScript.
