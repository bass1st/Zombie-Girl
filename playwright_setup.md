# Playwright Setup

## Installation

```bash
npm install -D playwright
npx playwright install
```

## Deterministic smoke command

Use the repository script below for deterministic smoke checks:

```bash
npm run test:smoke:playwright
```

Current script behavior:
- executes Playwright with `--workers=1 --retries=0 --reporter=line`
- targets `tests/smoke`
- is intended for quick vertical-slice transition checks

## Validation pipeline

Run this before PR creation:

```bash
npm run validate
```

This executes lint -> test -> build -> Playwright smoke in order.
