# Zombie Girl: Morrowsoil — Implementation Brief (Approved Concise)

## Product definition
- **Genre:** Story-driven tactical puzzle adventure (light action-RPG + light survival pressure).
- **Camera:** 2D top-down oblique / three-quarter view.
- **Player character:** **Lottie Harrow** (small zombie-born girl).
- **Core companions/tools:** **Nib** (crow companion), **Kindly** (oversized shotgun).

## Pillars (must stay true)
1. **Small body, big consequences** (size affects cover, movement, recoil, vulnerability).
2. **Zombie-born perspective** (not “monster seeking human approval”).
3. **One mechanic family everywhere** (exploration, puzzles, infiltration, combat).
4. **Eerie but warm** tone.
5. **Standalone clarity first**, deeper lore optional.

## Core loop
Explore → detect anomaly → solve traversal/puzzle → tactical encounter or escape → collect salvage/clue → return to safety/story gate → unlock next area.

## Core mechanics to implement first
- **Stillness:** corpse-like inert state for stealth, sensor bypass, aggro manipulation.
- **Scent:** lure/route manipulation + environmental interaction system.
- **Kindly/Recoil:** shotgun force logic (combat + traversal + puzzle interactions).
- **Nib:** scouting, small remote interactions, warning cues.

## MVP scope
- **Length:** 5–7 hours.
- **Structure:** Prologue + 5 chapters + final chapter.
- **Playable lead:** Lottie only.
- **Key regions:** Haywake, travel corridor, marsh/drowned zone, archive scar, Pale Quarter, Dawn Bell finale.
- **Out of scope:** open world, multiplayer, base building, giant crafting trees, party tactics, roguelike campaign, heavy rarity/stat systems.

## Combat model (encounter rooms)
- Real-time exploration, room-based tactical turn mode on trigger.
- Baseline turn: one move phase + **2 AP**.
- Typical AP costs: shoot/item/interact/stillness = 1 AP.
- Keep enemy counts low; prioritize readable “combat as puzzle.”

## Story spine
Lottie investigates wrong-death anomalies, discovers the Pale Quarter’s **Redemption** doctrine and **Dawn Bell** extinction plan, and stops mass erasure of surface zombie civilization.

## Primary implementation order
1. Exploration + room transition to tactical mode.
2. Stillness + recoil + one Nib interaction.
3. One anomaly puzzle room + one tactical room.
4. Dialogue return + checkpoint/save loop.

## Acceptance bar for MVP identity
A room is valid only if it meaningfully combines at least **two** of: movement, Stillness, Scent, Nib, Kindly/Recoil.
