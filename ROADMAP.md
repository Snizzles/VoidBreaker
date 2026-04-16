# VOID BREAKER — Roadmap

This document tracks planned features, improvements, and long-term design goals. Items are roughly ordered by priority within each section, not by release date.

---

## Near-Term (v1.x)

### Gameplay
- [x] **Pause menu** — ESC to pause/resume, overlay with resume button (v1.6.0)
- [ ] **Volume control** — mute toggle and basic slider in the overlay
- [x] **Difficulty modes** — Easy / Normal / Hard selectable at run start; each tunes enemy scaling, spawn rate, heart drops, healing, and Void Beast stats (v1.8.0)
- [ ] **Voidpossible mode** — a fourth difficulty beyond Hard; planned but not yet designed
- [ ] **Hard-mode unlocks** — clear Normal to unlock Void difficulty
- [x] **Key collection win condition** — collect 3 scattered keys before 10:00 to win; replaces pure survival timer (v1.4.0)
- [x] **Key difficulty rebalance** — keys spawn further out (1800-2800px) and are guarded by enemy clusters that spawn on approach (v1.5.0)
- [x] **Void Gate + Void Beast final boss** — collecting all 3 keys requires returning to origin and defeating the Void Beast (2500 HP, ranged crimson bolts) to win (v1.6.0)
- [x] **Phantom teleport fix** — minimum teleport distance increased from 60px to 140px so phantoms no longer land on top of the player (v1.6.0)
- [ ] **Run timer display improvement** — show a ghost timer comparing current run to personal best

### Weapons
- [ ] **Ricochet Round** — bullet that bounces off enemies up to N times, angle-reflected
- [ ] **Void Spike** — fires a single massive piercing beam in the direction of movement
- [x] **Combat Drones** — deploys auto-targeting mini-drones that orbit and track enemies independently (v2.0.0)

### Passives
- [ ] **Leech Core** — restore a small amount of HP per kill
- [ ] **Blast Radius** — increases explosion radius of Nova Bomb and any future AoE weapons
- [ ] **Overcharge** — first shot after standing still for 0.5s deals 2× damage

### Quality of Life
- [x] **Achievements** — local badge system (first boss kill, 5-minute survival, ×20 combo, etc.) (v1.7.0)
- [x] **Achievements on pause screen** — full achievement list with locked/unlocked status visible any time via ESC (v1.9.0)
- [x] **Continue Playing fix** — game correctly resumes after defeating the Void Beast instead of looping back to the end screen (v1.9.0)
- [x] **XP Magnet pickup** — rare world drop (1-2×/run) that pulls all XP gems to the player for 5 seconds (v1.9.2)
- [x] **XP vacuum on key collect** — collecting a key automatically pulls all on-screen XP gems to the player (v1.8.1)
- [ ] **Kill counter by enemy type** — end screen breakdown of what you killed
- [ ] **Damage summary** — per-weapon damage % chart on the end screen
- [ ] **Gem vacuum on boss kill** — auto-collect all on-screen gems when a boss dies
- [ ] **Minimap** — small corner display showing enemy density around the player
- [x] **Off-screen key indicators** — arrow + distance at screen edge pointing toward uncollected keys (v1.4.0)
- [ ] **Pending level-up counter** — show queued level-ups (e.g. "2 pending") on the XP bar when multiple are stacked
- [ ] **Weapon DPS display** — show estimated DPS next to each weapon in the weapons HUD

---

## Medium-Term (v2.x)

### Meta-Progression
- [ ] **Persistent currency** — earn "Void Shards" each run based on score, usable between runs
- [ ] **Unlock tree** — spend Void Shards to permanently unlock weapons/passives that appear more often, or start with a bonus stat
- [ ] **Run records** — save best time, highest score, and max combo per difficulty locally

### Stage 2: Defend Earth
- [x] **Stage 2 game mode** — 12-wave defense mode triggered after Stage 1 victory; Earth background; player keeps full build; massive enemy counts (v2.0.0)
- [x] **Attribute point system** — repeatable stat boosts (+5% Damage, +5% Speed, +15 Max HP, +3 Armor) when all weapon/passive upgrades are maxed (v2.0.0)
- [x] **Multi-Void Beast final wave** — 3 mobile Void Beasts in Wave 12 as the ultimate challenge (v2.0.0)
- [x] **Combat Drones available in Stage 2** — weapon slot cap raised 6→7 so a fully-armed Stage 1 player can still unlock Drones (v2.0.2)
- [x] **Stage 2 balance tuning** — wave HP scaling reduced 0.3→0.25; Gravity Vortex DPS buffed; Hard mode start HP raised 75→100 (v2.0.3)
- [x] **Stage 2 bug fixes** — enemy spawn distance pulled in (just off-screen); wave-clear waits for enemies to die; Wave 12 Void Beasts arrive within 6s (v2.0.5)
- [x] **Skip to Stage 2 — Full Build** — home screen button launches Stage 2 immediately with all weapons/passives maxed; Combat Drones available via in-game level-ups (v2.0.6)

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
- [x] **Sidney Mode** — Easy difficulty with no time limit and no boss spawns; relaxed exploration for players who want to grind builds without pressure (v1.9.1)
- [x] **Sidney Mode → Stage 2 portal** — Earth Portal waypoint at map origin glows green after 15s; walk into it to launch Stage 2 with your Sidney build (v2.0.4)
- [ ] **Endless mode** — no key/timer win condition; pure score chase with a global leaderboard
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
- [ ] **Custom soundtrack** — procedurally generated or looping chiptune tracks per arena theme
- [ ] **Accessibility options** — colorblind palette, reduced motion mode, larger UI text

---

## Known Issues / Tech Debt

- Star background uses `%` wrap math that produces minor visual stutter at large camera offsets — switch to true parallax tile wrapping
- No frame-rate independence guard beyond `dt` cap of 50ms — very low FPS devices may still exhibit physics jitter
- Enemy eye always faces right — should rotate toward the player's position for better visual feedback
- ~~No off-screen enemy indicators~~ — key indicators added in v1.4.0; boss/elite indicators still TODO
- No visual feedback for armor damage reduction — blocked damage should flash a shield icon or show reduced numbers in a distinct color

---

*This roadmap reflects current intentions and will change. Community feedback welcome via [GitHub Issues](../../issues).*
