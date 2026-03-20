# VOID BREAKER

A browser-based auto-shooter in the spirit of *Vampire Survivors* — survive endless waves of void creatures, collect XP gems, level up, and build a weapon loadout powerful enough to break the void.

**[▶ Play in browser](https://snizzles.github.io/VoidBreaker/)** &nbsp;·&nbsp; Single file, no install, no dependencies.

---

## How to Play

| Input | Action |
|-------|--------|
| `WASD` / Arrow Keys | Move |
| `Escape` | Pause / Resume |
| Touch left side of screen | Virtual joystick (mobile) |

Weapons fire **automatically** — your only job is to move.

**Goal:** Collect all 3 🔑 keys scattered across the map, return to the **Void Gate** at the center, and defeat the **Void Beast** final boss to escape the void — all before 10:00. Kill enemies → collect ◆ gems → fill XP bar → level up → pick upgrades to survive long enough.

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

The **Void Beast** is the final boss — it spawns at the Void Gate when you return with all 3 keys. It has massive HP and fires spreads of crimson bolts. Defeat it to win — or keep playing after victory for endless mode.

---

## Achievements

13 achievements tracked in your browser across all runs. Unlock notifications appear in-game when earned; your total is shown on the end screen.

| Achievement | How to unlock |
|-------------|---------------|
| 🩸 First Blood | Kill your first enemy |
| 💀 Void Slayer | Kill 100 enemies in one run |
| ☠️ Annihilator | Kill 500 enemies in one run |
| 👹 Boss Hunter | Kill your first boss |
| 🏆 Boss Slayer | Kill 3 bosses in one run |
| 🔑 Key Master | Collect all 3 keys |
| ✦ Void Breaker | Defeat the Void Beast |
| ⚡ Combo King | Reach a ×20 kill combo |
| ⬆️ Power Rising | Reach level 20 |
| 🌟 Ascended | Reach level 50 |
| ⏱️ Survivor | Survive for 5 minutes |
| 🔫 Arsenal | Equip 4 weapons simultaneously |
| 💥 Obliterator | Deal 100,000 total damage |

---

## Survival Tips

- **Move constantly.** Standing still lets enemies surround and overwhelm you.
- **Prioritize Bosses.** They drop large XP gem clusters worth many level-ups.
- **Synergize passives.** Chrono Chip + Chain Bolt or Power Core + Nova Bomb compound hard.
- **Kill streaks matter.** Combos multiply score — keep the chain going for bonus points.
- **Follow the arrows.** Off-screen key indicators point you toward uncollected keys with distance readouts.
- **Prepare for guardians.** Each key is defended by a Brute and a cluster of enemies that spawn when you get close.
- **Return to the Void Gate.** After collecting all 3 keys, a gold arrow guides you back to the map origin.
- **Defeat the Void Beast.** The final boss guards your escape — dodge its crimson bolts and finish it off to win.

---

## Technical

- Pure vanilla HTML/CSS/JS — single `index.html` file, zero dependencies
- Canvas 2D rendering with world-space camera
- Procedural audio via Web Audio API (no audio files)
- Touch-compatible with virtual joystick for mobile play

---

## Difficulty Modes

Choose your challenge at the start of each run:

| Difficulty | Starting HP | Enemy Scaling | Heart Drops | Void Beast HP |
|------------|-------------|---------------|-------------|---------------|
| Easy | 150 | Slow (cap 3×) | 10% chance, 28 HP | 250,000 |
| Normal | 100 | Standard (cap 7×) | 5% chance, 18 HP | 500,000 |
| Hard | 75 | Fast (cap 10×) | 2% chance, 10 HP | 1,000,000 |

---

## Version History

| Version | Notes |
|---------|-------|
| v1.8.0 | Difficulty modes: Easy / Normal / Hard; enemy scaling, heart drops, healing, and Void Beast stats all tuned per difficulty; max enemy cap raised to 200 |
| v1.7.0 | Achievements (13 badges, localStorage-persistent, in-game toast notifications); Void Beast massively buffed; Continue Playing button on win screen |
| v1.6.0 | Void Gate + Void Beast final boss; ESC pause menu; phantom teleport distance fix |
| v1.5.0 | Key difficulty rebalance: keys spawn 3× further out (1800-2800px); guardian enemies (elite Brute + Crawler/Swarm cluster) spawn to defend each key on approach |
| v1.4.0 | Performance overhaul (no shadowBlur, off-screen culling, enemy cap); key collection win condition; off-screen key indicators; auto-skip level-up when maxed; heal always offered |
| v1.3.0 | Performance pass; reduce round to 10 minutes |
| v1.2.1 | Shadow Orbs distinct gold color |
| v1.2.0 | Fix Chain Bolt off-screen kills; fix Nova Bomb damage multiplier |
| v1.1.0 | Starting weapon selection; version display |
| v1.0.0 | Initial release |

See [ROADMAP.md](ROADMAP.md) for planned features.
