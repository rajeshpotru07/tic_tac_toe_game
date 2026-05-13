# 7H Game Zone

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Single%20File-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-Vanilla%20ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/No%20Dependencies-Zero%20Install-00f5d4?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-7209b7?style=for-the-badge"/>
</p>

<p align="center">
  A cyberpunk-themed browser game portal — three AI-powered games, zero dependencies, one HTML file.
</p>

---

## 🎮 Games

| Game | Description | AI Type |
|---|---|---|
| ✕〇 **Tic Tac Toe** | Classic 3×3 grid, you vs AI | Rule-based heuristic |
| 🃏 **Card Wars** | Battle with the highest card | Randomized hand selection |
| ♟ **Chess** | Full chess with all standard rules | Minimax + Alpha-Beta pruning |

---

## ✨ Features

- **Custom callsign login** — personalized display throughout the session
- **Session scoreboards** — win/loss/tie counts per game, reset on new game
- **Cyberpunk aesthetic** — animated neon grid, glowing accents, Orbitron + Rajdhani fonts
- **Fully self-contained** — one `.html` file, no build tools, no frameworks, no npm
- **Works offline** — only Google Fonts requires a network connection

---

## 🚀 Quick Start

1. Download `index.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Enter your callsign and click **ENTER THE ARENA**
4. Pick a game and play

No install. No setup. Just open and play.

---

## 🕹️ How to Play

### ✕〇 Tic Tac Toe
You are **X**, AI is **O**. Click any empty cell to place your mark. The AI responds immediately using a priority strategy — it will try to win, then block you, then take the best available square.

### 🃏 Card Wars
Both sides are dealt **5 cards** from a shuffled 52-card deck (AI's hand stays face-down). Click any card in your hand to play it. The AI picks randomly from its hand. Higher card wins — Ace is highest, 2 is lowest. Draw extra cards or reset the deck anytime.

### ♟ Chess
Full rules apply: **castling**, **en passant**, **check/checkmate/stalemate**, and **pawn promotion** (auto-promotes to Queen). Click a piece to see its legal moves highlighted in green, then click a destination to move. Use **Undo** to take back your last move plus the AI's response.

---

## 🤖 Chess AI Details

The chess engine uses **Minimax search at depth 2** with **alpha-beta pruning** for performance.

Evaluation is based on:
- **Material value** — standard piece weights (Pawn 100, Knight 320, Bishop 330, Rook 500, Queen 900)
- **Piece-square tables** — positional bonuses that reward center control, active knights, developed bishops, and king safety

At depth 2 the AI plays reasonably but is beatable — good for casual games.

---

## 📁 File Structure

```
7h-game-zone/
└── index.html       # Entire app — HTML + CSS + JS (~500 lines)
```

No folders, no build output, no config files.

---

## 🛠️ Tech Stack

| Layer | Details |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 — custom properties, grid, flexbox, keyframe animations |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — Orbitron, Rajdhani |
| AI (TTT) | Rule-based heuristic |
| AI (Chess) | Minimax + alpha-beta pruning, depth 2, piece-square tables |
| AI (Card Wars) | Random card selection |

---

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| IE / Legacy | ❌ Not supported |

No polyfills needed. No ES2022+ features used.

---

## ⚠️ Known Limitations

- Chess AI is depth-2 only — strong players will beat it
- Pawn promotion always produces a Queen (no piece selection dialog)
- Game state is lost on page refresh — no persistence or save feature
- No multiplayer, accounts, or online functionality

---

## 🤝 Contributing

Contributions are welcome! Some ideas to get started:

- Increase chess AI depth or add difficulty levels
- Add pawn promotion piece selection
- Add localStorage for score persistence across sessions
- Add a new game to the portal

Fork the repo, make your changes, and open a pull request.

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

<p align="center">
  Developed with ❤️ by <strong>Rajesh</strong> &nbsp;|&nbsp; 7H Game Zone
</p>
