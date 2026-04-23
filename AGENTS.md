# AGENTS.md

## Operational Instructions

1. Use only these canonical inputs for planning and implementation context:
   - `PLAN.md`
   - `Notes/game_brief.md`
   - `docs/playtest_checklist.md`
2. Implement only the current milestone defined in the plan.
3. Do not add opportunistic scope expansions, stretch goals, or unrelated improvements.
4. Run all required pre-PR checks before opening a PR:
   - lint
   - tests
   - build
   - Playwright smoke
5. Stop immediately if any required check fails.
6. Do not continue implementation, polish, or PR preparation after a failed check.
7. Never modify `main` directly.
8. Perform all work on a feature branch or isolated worktree.
9. Update `PLAN.md` in the same PR whenever milestone status, tasks, or scope changes.
10. Update every changed documentation file in the same PR as its related code change.
11. Keep MVP feature scope constrained.
12. Allowed MVP examples: core single-player loop, required UI flows, milestone-specific bug fixes, checklist-driven polish.
13. Forbidden MVP examples: open-world systems, multiplayer/networked play, live-service backends, economy overhauls, major content expansions, speculative refactors.
14. End every agent run with this exact output structure:
    - Summary
    - Files changed
    - Checks run
    - Risks
    - Next tiny step
