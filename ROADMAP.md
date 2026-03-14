# VOID BREAKER — Roadmap

This document tracks planned features, improvements, and long-term design goals. Items are roughly ordered by priority within each section, not by release date.

---

## Near-Term (v1.x)

### Gameplay
- [ ] **Pause menu** — allow pausing mid-run with keybind (Escape)
- [ ] **Volume control** — mute toggle and basic slider in the overlay
- [ ] **Difficulty modes** — Easy / Normal / Void (harder). Void mode scales enemies more aggressively and disables hearts
- [ ] **Hard-mode unlocks** — clear Normal to unlock Void difficulty
- [ ] **Run timer display improvement** — show a ghost timer comparing current run to personal best

### Weapons
- [ ] **Ricochet Round** — bullet that bounces off enemies up to N times, angle-reflected
- [ ] **Void Spike** — fires a single massive piercing beam in the direction of movement
- [ ] **Drone Swarm** — deploys auto-targeting mini-drones that orbit at long range and track enemies independently

### Passives
- [ ] **Leech Core** — restore a small amount of HP per kill
- [ ] **Blast Radius** — increases explosion radius of Nova Bomb and any future AoE weapons
- [ ] **Overcharge** — first shot after standing still for 0.5s deals 2× damage

### Quality of Life
- [ ] **Kill counter by enemy type** — end screen breakdown of what you killed
- [ ] **Damage summary** — per-weapon damage % chart on the end screen
- [ ] **Gem vacuum on boss kill** — auto-collect all on-screen gems when a boss dies
- [ ] **Minimap** — small corner display showing enemy density around the player
- [ ] **Off-screen boss/elite indicator** — arrow or icon at screen edge pointing toward approaching bosses
- [ ] **Pending level-up counter** — show queued level-ups (e.g. "2 pending") on the XP bar when multiple are stacked
- [ ] **Weapon DPS display** — show estimated DPS next to each weapon in the weapons HUD

---

## Medium-Term (v2.x)

### Meta-Progression
- [ ] **Persistent currency** — earn "Void Shards" each run based on score, usable between runs
- [ ] **Unlock tree** — spend Void Shards to permanently unlock weapons/passives that appear more often, or start with a bonus stat
- [ ] **Run records** — save best time, highest score, and max combo per difficulty locally

### New Content
- [ ] **2 new boss types**
  - *Fragmenter* — splits into 4 smaller mini-bosses when hit below 50% HP
  - *The Mirror* — copies the player's current dominant weapon type and uses it against them
- [ ] **Elite enemies** — rare gold-outlined variants of existing types with 3× HP and a special ability (Darter elite dashes; Brute elite ground-slams)
- [ ] **Event waves** — occasional timed scripted waves ("SWARM SURGE — 20 seconds of only Swarm enemies") with bonus XP on completion
- [ ] **Weapon synergy bonuses** — equipping specific pairs of weapons unlocks a passive bonus (e.g. Laser Whip + Gravity Vortex → enemies in vortex take 30% more whip damage)

### World
- [ ] **Arena themes** — cosmetic background variants (Neon City, Deep Space, Blood Moon) selectable at run start
- [ ] **Environmental hazards** — arena-mode obstacles: void rifts that teleport the player, plasma walls that periodically sweep the arena

---

## Long-Term (v3.x+)

### Game Modes
- [ ] **Endless mode** — no 20-minute win condition; pure score chase with a global leaderboard
- [ ] **Challenge runs** — pre-set loadouts with specific win conditions ("Survive 5 minutes with only Shadow Orbs and no passives")
- [ ] **Daily run** — seeded random loadout that resets every 24h, shared score board

### Weapons & Builds
- [ ] **Weapon evolution system** — reaching max level on a weapon + owning a specific passive transforms it into an evolved form (inspired by Vampire Survivors)
  - Void Pulse + Power Core → **Void Nova** (pulses explode on contact)
  - Laser Whip + Chrono Chip → **Plasma Hurricane** (dual counter-rotating beams)
  - Chain Bolt + Magnet Field → **Arc Field** (continuous electrical aura)
  - Nova Bomb + Blast Radius → **Singularity Cannon** (massive single nuke per wave)
  - Shadow Orbs + Phase Drive → **Phase Blades** (orbs leave trailing damage zones)
  - Gravity Vortex + Void Shield → **Event Horizon** (inverts pull into a repulsion burst)
- [ ] **Cursed upgrades** — optional high-risk/high-reward cards at level-up: double damage but take 50% more hits, or gain 3 weapon levels but lose 40 max HP

### Polish
- [ ] **Animated title screen** — particle void effect on the main overlay
- [ ] **Death replay** — short 3-second instant replay of the killing blow
- [ ] **Achievements** — local badge system (first boss kill, 10-minute survival, x20 combo, etc.)
- [ ] **Custom soundtrack** — procedurally generated or looping chiptune tracks per arena theme
- [ ] **Accessibility options** — colorblind palette, reduced motion mode, larger UI text

---

## Known Issues / Tech Debt

- Star background uses `%` wrap math that produces minor visual stutter at large camera offsets — switch to true parallax tile wrapping
- No frame-rate independence guard beyond `dt` cap of 50ms — very low FPS devices may still exhibit physics jitter
- Enemy eye always faces right — should rotate toward the player's position for better visual feedback
- No off-screen enemy indicators — large enemies or bosses approaching from outside the viewport give no warning
- No visual feedback for armor damage reduction — blocked damage should flash a shield icon or show reduced numbers in a distinct color

---

*This roadmap reflects current intentions and will change. Community feedback welcome via [GitHub Issues](../../issues).*
