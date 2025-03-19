# 🎮 TIC TAC TOE - Python Edition

> *"A classic game, reimagined in the console with AI and multiple modes!"*



---

## 📜 Description

This is a fully interactive **Tic Tac Toe game** built using **Python**, playable in your terminal/console!  
Choose between:
- 👥 Player vs Player
- 🧠 Player vs Computer
- 🤖 Computer vs Computer (Fast simulation!)

The game includes smart AI, clean board visuals, and friendly prompts to ensure a smooth and engaging experience.

---

## 🧠 Features

- 🎮 Three Game Modes (PvP, PvC, CvC)
- ✅ Smart AI with strategy (block win, take win, pick corners)
- 🧾 User-friendly UI with board & guide
- 🌀 Random turn chooser
- 🔁 Replayable loop
- 💡 Input validation & helpful prompts

---

## 🕹️ Game Board Reference
## 🔄 Game Flowchart

```mermaid
flowchart TD
    A[Start Game] --> B{Select Mode}
    B --> C[Player vs Player]
    B --> D[Player vs AI]
    
    C --> E[Display Empty Board]
    D --> E

    E --> F{Whose Turn?}
    F --> G[Player 1 Input]
    F --> H[Player 2 / AI Input]

    G --> I[Update Board]
    H --> I
    I --> J[Check Win / Draw]

    J -->|Win| K[Show Result: Winner]
    J -->|Draw| L[Show Result: Draw]
    J -->|Continue| F

    K --> M[Restart or Exit]
    L --> M

