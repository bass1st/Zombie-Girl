# B — Update Plan Prompt Template

## Purpose
Use this prompt to update `PLAN.md` so it reflects the latest execution loop state for the **current milestone only**.

## Required input files
- `PLAN.md`
- `Notes/game_brief.md`
- `docs/playtest_checklist.md`

## Explicit allowed scope
- Update milestone status, blockers, and task progress in `PLAN.md`.
- Align plan wording with current accepted milestone constraints.
- Keep acceptance criteria and command categories explicit and testable.

## Forbidden scope expansion
- Do **not** add new milestones or broaden MVP scope.
- Do **not** introduce unrelated backlog items or speculative architecture changes.
- Do **not** modify design intent beyond what current canonical inputs require.

## Required validation commands
Run and report:
- `npm run lint`
- `npm test`
- `npm run build`
- `npx playwright test --grep "vertical slice identity loop"`

If necessary, substitute project-native equivalents for each required category.

## Output format
Return exactly these sections:
1. `Status`
2. `Diffs`
3. `Failures`
4. `Next step`

Section guidance:
- **Status:** whether plan update is complete and internally consistent.
- **Diffs:** specific `PLAN.md` changes made.
- **Failures:** failed checks or unresolved plan contradictions.
- **Next step:** one tiny, milestone-safe action.
