# Jay Lorona — Full-Stack Game Developer & Builder

Solo developer shipping production-quality games, arcade platforms, and backend infrastructure. Every piece built to solve a real problem, not to learn a framework.

→ **[jayarcade.com](https://jayarcade.com)** | **[factory.jayarcade.com](https://factory.jayarcade.com)**

---

## Flagship Projects

**Tactical Arena** — Isometric squad tactics game (Play Store release candidate)
- 30-unit roster with ARTS/passives/statuses/summons/weather/terrain mechanics
- 22-mission campaign with progression, objectives, and reward choices
- Local hot-seat (2–4P FFA/teams), CPU matches (3 difficulties), and online Versus (Classic/Draft/FFA/Teams)
- Server-authoritative Ranked 1v1 matchmaking with ELO
- Deterministic headless rules engine with full test coverage
- Android build with Google Play Billing and social platform integration
- Packaged at `/mobile/tactical-arena/` — ready for production
- **[Core game code](https://github.com/loronajay/javascript-game-factory/tree/main/games/tactical-arena)** • **[Mobile build](https://github.com/loronajay/javascript-game-factory/tree/main/mobile/tactical-arena)**

**JavaScript Game Factory** — Production arcade platform (11 released titles)
- Complete tech stack: TypeScript frontend + Node.js backend, global leaderboards, social/identity layer
- 13 shipped cabinets: Tactical Arena, Sumorai, Mini-Tactics, Illuminauts, Cockpit Swarm, Bird Duty, Creature Battler, Battleships, Circuit Siege, Echo Duel, Build Buddy, Lovers Lost, Speed Demon
- Server-authoritative online play with rollback netcode, ranked matchmaking, account progression
- Deterministic core engines with comprehensive test harnesses (online sync, campaign logic, AI)
- **[Live at factory.jayarcade.com](https://factory.jayarcade.com)**

**Other Games in Development**
- Sumorai — 1v1 rollback netcode fighter with ranked ELO
- Mini-Tactics — 2–4P tactical squad battles with lockstep online
- Cockpit Swarm — 3D fixed-shooter with 15-stage campaign
- Circuit Siege — Server-authoritative 1v1 route-repair strategy game
- Build Buddy — Co-op platformer with role-specific multiplayer

---

## Infrastructure & Backend

**Jay Arcade Platform**
- [leaderboard-server](https://github.com/loronajay/leaderboard-server) — Global leaderboards (REST API + PostgreSQL on Railway)
- [factory-network-server](https://github.com/loronajay/factory-network-server) — WebSocket server: matchmaking, room management, peer messaging
- Python build pipeline for game extraction, patching, analytics injection, deployment
- Platform features: account identity, player profiles, social graph, notifications, player activity feeds

**Hardware & Embedded**
- [bird-duty-lite](https://github.com/loronajay/bird-duty-lite) — ESP32 handheld gaming "playable business card"

---

## How I Work

I build with AI assistance—modularly, with understanding at each step.
I think in systems: how pieces connect, where failure points are, what to automate.
When something is painful to repeat, I build a tool so I never repeat it.

**Strongest at:** Shipping production games end-to-end, deterministic game logic, online sync/netcode, backend infrastructure, test-driven game development, identifying and solving real problems.

---

## Tech Stack

- **Frontend:** TypeScript, vanilla HTML/CSS/JavaScript, canvas/WebGL
- **Backend:** Node.js, REST APIs, WebSocket servers, PostgreSQL
- **Game Logic:** Deterministic reducers, Node test harnesses, rollback netcode
- **Mobile:** Capacitor, Google Play Billing
- **Embedded:** ESP32, Arduino
- **Build & Automation:** Python, GitHub Actions
- **AI Integration:** LLM-assisted development workflows

---

**Email:** leojaylorona@gmail.com
