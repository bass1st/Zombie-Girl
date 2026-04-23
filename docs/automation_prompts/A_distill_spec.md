# A — Distill Spec Prompt Template

## Purpose
Use this prompt to produce a concise, implementation-ready spec distillation for the **current milestone only**.

## Required input files
- `PLAN.md`
- `Notes/game_brief.md`
- `docs/playtest_checklist.md`

## Explicit allowed scope
- Distill the active milestone into actionable bullets.
- Clarify acceptance criteria and validation expectations already present in the source files.
- Summarize blockers/risks that directly affect current milestone delivery.

## Forbidden scope expansion
- Do **not** propose new features, systems, regions, or mechanics outside the current milestone.
- Do **not** rewrite project vision, genre direction, or long-term roadmap.
- Do **not** add speculative refactors or unrelated polish work.

## Required validation commands
Run and report these categories before handoff:
- `npm run lint`
- `npm test`
- `npm run build`
- `npx playwright test --grep "vertical slice identity loop"`

If project commands differ, replace with repo-native equivalents while preserving categories: lint, tests, build, Playwright smoke.

## Output format
Return exactly these sections:
1. `Status`
2. `Diffs`
3. `Failures`
4. `Next step`

Section guidance:
- **Status:** pass/fail summary for milestone understanding.
- **Diffs:** what was distilled/clarified (no implementation changes).
- **Failures:** missing inputs, ambiguities, or failed validation commands.
- **Next step:** one smallest actionable follow-up.
