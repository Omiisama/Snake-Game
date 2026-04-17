# 🐍 Snake Game with Analytics Backend

A feature-rich Snake game built using **HTML5 Canvas and JavaScript**, enhanced with multiple game modes, smooth animations, and responsive controls.  
Includes a **Flask backend** for logging gameplay data and a **Bash-based admin tool** for log analysis using Unix utilities.

---

## Features

### Gameplay
- Smooth, animated snake movement with interpolation
- Multiple game modes:
  - **Normal** – classic gameplay  
  - **Wrapped** – snake passes through walls  
  - **Ghost** – snake can pass through itself  
- Dynamic speed settings (Slow → Hell Mode)
- Adjustable grid size
- Responsive controls:
  - Keyboard (WASD / Arrow keys)
  - Touch support (mobile swipe)

---

### UI/UX
- Animated food with pulse effect
- Gradient buttons with hover effects
- Pause / Resume functionality
- Polished Game Over screen with animations
- Demo snake on start screen

---

### Backend (Flask)
- REST API to save game data:
  - Name
  - Score
  - Duration
  - Speed
  - Game mode
  - Cause of death
  - Grid size
- Data stored in a flat file (`history.txt`)
- Input validation and error handling

---

### Admin Tool (Bash)
Menu-driven script to manage logs:

- Select user-specific data
- View recent games (paginated)
- View analytics:
  - Mean score
  - Average survival time
  - Death distribution
- Delete entries:
  - By username
  - By timestamp
  - Malformed entries
- Sort logs:
  - By timestamp
  - By username
  - By score
- Log rotation with compression

Uses:
- `awk`, `sed`, `grep`, `sort`, `tail`

---

## Tech Stack

- Frontend: JavaScript, HTML5 Canvas  
- Backend: Python (Flask)  
- Scripting: Bash  
- Storage: Flat file (`history.txt`)  

---
