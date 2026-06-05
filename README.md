# 🏁 Trackdown

> Race. Record. Analyze. Improve.

Trackdown is a browser-based racing game meets telemetry analytics platform. You pick a track, race 3 laps, and get a full breakdown of your performance compared against an AI model that drives the mathematically optimal racing line — hitting every apex, braking at the right point, and carrying maximum speed through every corner.

The gap between you and the model isn't just a time difference. It's a story told in data.

---

## The Idea

Most racing games tell you *that* you lost time. Trackdown tells you *where*, *why*, and *by how much*.

After each session, you get a side-by-side comparison of your driving vs the AI model across speed traces, corner entries, apex accuracy, braking zones, and straight-line acceleration. Over time, that data feeds back into improving the model itself — more players, better data, smarter AI.

The project has two sides to it:

- **The Game** — a retro NFS-inspired interface where you select tracks or draw your own, then race and get timed across 3 laps
- **The Analytics** — a telemetry dashboard that breaks down exactly where you're losing and gaining time versus the optimal line

---

## Features (Planned)

- 🎮 Browser racing game with classic track selection UI
- ✏️ Draw your own track and race it
- 👻 Ghost car showing the AI's optimal racing line
- 📊 Post-race analytics dashboard — speed traces, corner breakdown, sector deltas
- 🤖 Algorithmic racing line model (apex detection + optimal path)
- 🏆 Leaderboards per track
- 👤 Guest mode, with Google login coming later

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Game Engine | Phaser.js |
| Frontend | HTML / CSS / JavaScript |
| Backend | Python + FastAPI |
| Database | PostgreSQL |
| Analytics | Pandas, NumPy |
| Machine Learning | Scikit-Learn, XGBoost → PyTorch (later) |
| Visualization | Plotly |
| ML Tracking | MLflow |
| Auth | Guest mode → Firebase Auth (Google) |
| Deployment | Docker + Render / AWS |

---

## Status

🚧 This project is just getting started. This README will grow as the build progresses.

---

## Motivation

This started as a data science project. I wanted to build something that generates real, meaningful driving telemetry — not from a dataset someone else collected, but from actual users playing an actual game. The racing game is the data collection mechanism. The analytics and ML model are what make that data useful.

Eventually the goal is a model that doesn't just drive the geometric ideal, but learns from thousands of player sessions to understand *how different kinds of drivers lose time* — and give personalized recommendations to fix it.

---

*Built with Python, Phaser.js, and a genuine interest in why I keep losing time in sector 2.*
