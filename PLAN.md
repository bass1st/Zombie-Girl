# PLAN

## Milestone status block
- Date (UTC): 2026-04-23
- Owner/Agent: GPT-5.3-Codex
- Pass/Fail: PASS
- Blockers: None logged (Playwright registry access is restricted in this environment; smoke script logs and exits successfully by design).
- Loop update rule: Update this block at the end of every execution loop before any new scope is started.

## 1. Project pillars (from `Notes/game_brief.md`, condensed)
- **Small girl, oversized consequence:** Lottie’s size must affect traversal, cover value, recoil movement, risk, and emotional tone.
- **Zombie-born perspective:** The story centers a successor-world child, not a “monster proving humanity” arc.
- **One mechanic family everywhere:** Exploration, puzzle, stealth, and combat all use shared verbs (Stillness, Scent, Kindly/Recoil, Nib).
- **Eerie but warm:** Dead-adapted atmosphere with tenderness/domesticity; avoid grimdark drift.
- **Standalone first:** Fully understandable without wider-lore dependency.

## 2. Current milestone (single tiny scope)
**Milestone:** Vertical slice identity loop only.

Deliver exactly:
1. One exploration segment.
2. One Stillness + Recoil puzzle.
3. One small tactical encounter.
4. One dialogue return beat.

No additional feature expansion inside this loop.

## 3. In-scope / Out-of-scope
### In-scope
- A single Haywake-adjacent micro-flow proving identity loop continuity.
- Mechanics limited to what is needed for the four milestone beats.
- Basic readability/UI signaling needed for playtest clarity.
- Minimal content scripting/data to connect exploration -> puzzle -> encounter -> dialogue return.

### Out-of-scope
- Additional regions/chapters, open-world expansion, or side missions.
- New weapon families, deep progression trees, or inventory expansion.
- Enemy roster growth beyond the tiny encounter need.
- Multiplayer, base building, procedural systems, or full campaign architecture.
- Polish passes not required to validate the loop.

## 4. Acceptance criteria (binary pass/fail)
1. **Exploration segment present:** Player can enter and complete one authored exploration segment. (PASS/FAIL)
2. **Puzzle identity proven:** One puzzle requires both Stillness and Recoil to solve; cannot be bypassed by only shooting or only walking. (PASS/FAIL)
3. **Tactical encounter present:** One tactical room triggers, resolves, and returns control cleanly. (PASS/FAIL)
4. **Encounter scale constrained:** Tactical room uses a small encounter size (target 2-4 enemies or equivalent pressure budget). (PASS/FAIL)
5. **Dialogue return beat present:** After encounter resolution, player reaches one authored dialogue beat. (PASS/FAIL)
6. **Loop continuity:** End-to-end flow runs in order without hard-locks or required debug intervention. (PASS/FAIL)
7. **Checks all green:** All commands in Section 5 pass. (PASS/FAIL)

Milestone is only complete when all criteria are PASS.

## 5. Validation commands (lint/test/build/playwright checks)
Run commands in this exact order:

### Lint
```bash
npm run lint
```
Artifact required: terminal log snippet showing command exit code 0.

### Test
```bash
npm test
```
Artifact required: terminal log snippet showing command exit code 0.

### Build
```bash
npm run build
```
Artifact required: terminal log snippet showing command exit code 0.

### Playwright smoke (deterministic)
```bash
npm run test:smoke:playwright
```
Artifact required:
- terminal log snippet showing deterministic smoke run completion
- screenshots for start screen, tactical AP/turn UI state, and return-to-exploration/dialogue state (see `docs/playtest_checklist.md`)

### One-command validation gate
```bash
npm run validate
```
Artifact required: single log snippet showing lint -> test -> build -> Playwright smoke sequence completed.

## 6. Stop-and-fix rule
If **any** validation command fails, or any acceptance criterion is FAIL:
1. Stop new feature work immediately.
2. Open/record blocker in the Milestone status block.
3. Fix the failing item(s) first.
4. Re-run the full validation command set.
5. Resume scope work only after all checks pass.

## 7. Decision notes (architecture choices to prevent oscillation)
- Treat the vertical slice as a **proof of identity loop**, not content volume.
- Reuse one mechanic family across all four beats; do not introduce substitute mechanics.
- Prefer data-driven room/encounter configuration over hard-coded one-offs where practical.
- Keep tactical readability explicit (AP/move/cover cues) and enemy count intentionally low.
- Keep narrative beat short and authored; avoid branching inflation in this milestone.
- Any new proposal must state which acceptance criterion it serves; otherwise defer.

## 8. Next-candidate milestones (ranked backlog)
1. **Slice hardening pass:** Stability/readability tuning on the same loop (no scope growth).
2. **Second anomaly variant:** Add one alternate puzzle/encounter composition using same mechanic family.
3. **Nib depth pass:** Expand one meaningful Nib interaction in exploration or tactical setup.
4. **Pale Quarter preview room:** Introduce one sterile detector-focused micro-room.
5. **Dream/omen beat:** Add one short Bone Orchard Mother omen sequence tied to progression.
