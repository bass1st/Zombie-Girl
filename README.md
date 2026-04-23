# Zombie-Girl Factory Onboarding

This README is the canonical onboarding source for both human contributors and coding agents working in this repository.

## 1) Project purpose and MVP identity

**Project:** *Zombie Girl: Morrowsoil*  
**Purpose:** Deliver a compact, memorable MVP that proves the game’s core identity loop (not full production scope).

The MVP identity centers on:
- A small, zombie-born protagonist perspective.
- One shared mechanic family across exploration, puzzles, and tactical encounter spaces.
- A single, end-to-end vertical slice loop:
  1. exploration segment,
  2. Stillness + Recoil puzzle,
  3. small tactical encounter,
  4. dialogue return beat.

If a task does not directly help validate this loop, defer it.

## 2) “How this factory works” diagram

```text
raw notes
   -> distilled docs
      -> PLAN milestone
         -> implementation
            -> Playwright
               -> PR review
                  -> next loop
```

## 3) Required files and authority order

Use these inputs as planning and implementation authority, in this order:

1. `AGENTS.md` (operational constraints and workflow rules)
2. `PLAN.md` (active milestone, acceptance criteria, validation commands)
3. `Notes/game_brief.md` (project design identity and MVP intent)
4. `docs/playtest_checklist.md` (smoke/playtest validation expectations)

When in doubt, prefer the highest authority file above and stay inside current milestone scope.

## 4) Local run commands (setup, lint, test, smoke)

Run from repository root.

### Setup
```bash
npm install
npx playwright install --with-deps
```

### Lint
```bash
npm run lint
```

### Test
```bash
npm test
```

### Build
```bash
npm run build
```

### Playwright smoke
```bash
npx playwright test --grep "vertical slice identity loop"
```

## 5) Milestone operating procedure (start, validate, close)

### Start
1. Confirm you are not on `main`.
2. Read `PLAN.md` current milestone and acceptance criteria.
3. Implement only milestone-required work.

### Validate
1. Run all required checks, in order:
   - lint
   - tests
   - build
   - Playwright smoke
2. If any check fails: **stop immediately**, log blocker in `PLAN.md`, fix, then rerun full check set.

### Close
1. Verify all acceptance criteria are PASS.
2. Update `PLAN.md` milestone status block (date, pass/fail, blockers).
3. Prepare PR with required summary content (below).

## 6) PR expectations (what must be included in summary)

Every PR summary must include:
- **What changed:** concise description of implemented milestone tasks.
- **Why it changed:** which milestone acceptance criteria each change supports.
- **Validation results:** lint, test, build, and Playwright smoke outcomes.
- **Scope statement:** confirmation that no out-of-scope expansion was introduced.
- **Risk + next step:** known risks and the next smallest milestone-safe follow-up.

Keep PRs milestone-focused, auditable, and loop-ready.
