# Jay Lorona — Jay Arcade Portfolio

  Solo developer building a full-stack competitive arcade platform from the ground up.
  Every piece of infrastructure here was built to solve a specific real problem.

  → **[jayarcade.com](https://jayarcade.com)**

  ---

  ## The Ecosystem

  Jay Arcade
  ├── jayarcade.com               — game delivery platform, CRT frontend, 9 shipped titles
  ├── leaderboard-server          — REST API + PostgreSQL (Railway), per-game secret key auth
  ├── factory-network-server      — WebSocket server: rooms, matchmaking, peer messaging
  ├── build pipeline              — Python: ZIP extract → HTML patch → grid regenerate → deploy
  ├── jay-mobile.js               — custom on-screen arcade controller (d-pad + face buttons)
  └── TurboWarp Game Factory      — 11 modular extensions + AI game dev tooling
      ├── factory-leaderboards.js — score submission + leaderboard display, plug into any game
      ├── factory-network.js      — multiplayer in a few block calls
      ├── textify-blockify-IR     — serialize Scratch blocks → AI → render back as blocks
      └── + 8 more extensions     — physics, animation, camera, UI, audio, controls...

  Hardware in progress:
  └── bird-duty-lite              — ESP32 handheld "playable business card" (firmware pending)

  ---

  ## Why each piece exists

  **Leaderboard server** — Implementing leaderboards directly in TurboWarp games was messy
  and one-off every time. I needed something I could drop into any game without rebuilding
  the infrastructure. I built a REST API server with per-game authentication, then wrapped
  it in `factory-leaderboards.js` — a TurboWarp extension that makes score submission a
  single block call.

  **Build pipeline** — I was manually editing HTML for every game export. By game #3 that
  was unsustainable. I wrote a Python pipeline that handles extraction, patching, analytics
  injection, and grid regeneration automatically.

  **Factory Network** — Adding multiplayer to a TurboWarp game meant understanding
  WebSocket servers, room management, and matchmaking from scratch. I built the server
  and a companion extension so that multiplayer is a few block calls, not an
  infrastructure project.

  **Textify/Blockify IR** — I couldn't get useful AI assistance with TurboWarp block
  programs because there was no way to express block logic as text. I designed a
  round-trip IR system: serialize blocks to a canonical text format → send to AI →
  render the result back as visual Scratch blocks.

  ---

  ## How I work

  I build with AI assistance — modularly, with understanding at each step.
  I think in systems: how pieces connect, where failure points are, what to automate.
  When something is painful to repeat, I build a tool so I never repeat it.

  Strongest at: system design, build tooling, end-to-end product shipping,
  identifying real problems and building real solutions.

  ---

  ## Repos

  | Repo | What it is |
  |---|---|
  | [textify-blockify-IR](https://github.com/loronajay/textify-blockify-IR) | TurboWarp Game Factory — extensions + IR
  tooling |
  | [factory-network-server](https://github.com/loronajay/factory-network-server) | WebSocket matchmaking server |
  | [leaderboard-server](https://github.com/loronajay/leaderboard-server) | Global leaderboard REST API |
  | [bird-duty-lite](https://github.com/loronajay/bird-duty-lite) | ESP32 handheld hardware project |
  | [games-directory-page](https://github.com/loronajay/games-directory-page) | jayarcade.com — the platform |

  **Email:** leojaylorona@gmail.com
