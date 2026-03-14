# VOID BREAKER

A browser-based auto-shooter in the spirit of *Vampire Survivors* — survive endless waves of void creatures, collect XP gems, level up, and build a weapon loadout powerful enough to break the void.

**[▶ Play in browser](https://snizzles.github.io/VoidBreaker/)** &nbsp;·&nbsp; Single file, no install, no dependencies.

---

## How to Play

| Input | Action |
|-------|--------|
| `WASD` / Arrow Keys | Move |
| Touch left side of screen | Virtual joystick (mobile) |

Weapons fire **automatically** — your only job is to move.

**Goal:** Collect all 3 🔑 keys scattered across the map before 10:00 to break the void. Kill enemies → collect ◆ gems → fill XP bar → level up → pick upgrades to survive long enough.

---

## Weapons

| Weapon | Description |
|--------|-------------|
| 💥 Void Pulse | Fires bursts of pulses in all directions |
| ⚡ Laser Whip | Rotating energy beam that sweeps nearby enemies |
| 💣 Nova Bomb | Drops explosive charges with AoE blast radius |
| 🔗 Chain Bolt | Lightning that chains between multiple enemies |
| 🌑 Shadow Orbs | Orbiting damage spheres that circle the player |
| 🌀 Gravity Vortex | Pulls enemies inward and deals continuous damage |

Each weapon has 8 upgrade levels unlocked through the level-up system.

## Passive Upgrades

| Passive | Effect |
|---------|--------|
| ⚡ Power Core | All weapons deal more damage |
| 💨 Phase Drive | Move faster |
| ❤️ HP Matrix | Increase max health (also heals) |
| 🧲 Magnet Field | Pull XP gems from further away |
| ⏱️ Chrono Chip | All weapons fire faster |
| 🛡️ Void Shield | Reduce damage taken per hit |

## Enemies

| Enemy | Behavior |
|-------|----------|
| Crawler | Basic slow-moving pursuer |
| Darter | Fast and fragile |
| Brute | Tanky and hard-hitting |
| Phantom | Teleports near the player |
| Swarm | Weak but spawns in large numbers |
| Leaper | Lunges toward the player periodically |

Bosses spawn every 2 minutes: **Void Titan**, **Eclipse Horror**, and **Singularity**.

---

## Survival Tips

- **Move constantly.** Standing still lets enemies surround and overwhelm you.
- **Prioritize Bosses.** They drop large XP gem clusters worth many level-ups.
- **Synergize passives.** Chrono Chip + Chain Bolt or Power Core + Nova Bomb compound hard.
- **Kill streaks matter.** Combos multiply score — keep the chain going for bonus points.
- **Follow the arrows.** Off-screen key indicators point you toward uncollected keys with distance readouts.
- Collect all 3 keys before 10:00 to win.

---

## Technical

- Pure vanilla HTML/CSS/JS — single `index.html` file, zero dependencies
- Canvas 2D rendering with world-space camera
- Procedural audio via Web Audio API (no audio files)
- Touch-compatible with virtual joystick for mobile play

---

## Version History

| Version | Notes |
|---------|-------|
| v1.4.0 | Performance overhaul (no shadowBlur, off-screen culling, enemy cap); key collection win condition; off-screen key indicators; auto-skip level-up when maxed; heal always offered |
| v1.3.0 | Performance pass; reduce round to 10 minutes |
| v1.2.1 | Shadow Orbs distinct gold color |
| v1.2.0 | Fix Chain Bolt off-screen kills; fix Nova Bomb damage multiplier |
| v1.1.0 | Starting weapon selection; version display |
| v1.0.0 | Initial release |

See [ROADMAP.md](ROADMAP.md) for planned features.
