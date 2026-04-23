# C — Implement and Verify Prompt Template

## Purpose
Use this prompt to implement only the current milestone slice and verify it with required checks.

## Required input files
- `PLAN.md`
- `Notes/game_brief.md`
- `docs/playtest_checklist.md`

## Explicit allowed scope
- Implement tasks that directly satisfy current milestone acceptance criteria.
- Apply checklist-driven fixes needed to pass milestone validation.
- Update related docs in the same run when implementation changes behavior.

## Forbidden scope expansion
- Do **not** start new systems outside milestone acceptance criteria.
- Do **not** add content expansions (new chapters/regions/mechanics) not required by current loop.
- Do **not** perform speculative refactors, broad rewrites, or non-blocking polish sprees.

## Required validation commands
Run and report all required categories:
- `npm run lint`
- `npm test`
- `npm run build`
- `npx playwright test --grep "vertical slice identity loop"`

If native commands differ, map each category to its repo-native equivalent and report the exact command used.

## Output format
Return exactly these sections:
1. `Status`
2. `Diffs`
3. `Failures`
4. `Next step`

Section guidance:
- **Status:** implementation and verification outcome.
- **Diffs:** code/docs changed, grouped by intent.
- **Failures:** failing checks, blockers, or unmet acceptance criteria.
- **Next step:** smallest unblock or completion action.
