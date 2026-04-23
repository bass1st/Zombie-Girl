# Zombie-Girl

zombie girl indie game development.

## Package scripts

```bash
npm run lint
npm test
npm run build
npm run test:smoke:playwright
npm run validate
```

- `test:smoke:playwright`: deterministic smoke command (single worker, no retries) for vertical-slice checks.
- `validate`: runs lint -> test -> build -> Playwright smoke in order.

## Build/validation artifacts

Validation evidence is required for PRs:
- terminal log snippets for each command
- screenshots/log snippets described in `docs/playtest_checklist.md`
