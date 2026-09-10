# AGENTS.md

Spec-first repo, no code on any branch. `README.md` (ES) is the spec: vehicle journal ("bitácora del vehículo"), localStorage-only, no backend; target stack React + Vite + Tailwind + TS on Vercel; branches main/dev + PR template.

- Package manager is pnpm (`packageManager` pinned in `package.json`, lockfile `pnpm-lock.yaml`). Target scripts per README: `pnpm run dev|check|build|lint` (currently placeholder stubs, green until the real scaffold lands); pre-commit gate `pnpm run check && pnpm run build && pnpm run lint`. CI (`.github/workflows/ci.yml`) runs the same gate on every PR and push to main/dev. Do not invent others.
- Keep docs/UX copy in Spanish unless asked otherwise (README is Spanish); code and PRs in English. User strings ship in ES in the same commit as the UI that uses them; keep the t() skeleton and Lang type for future EN, no dead ES keys.
- Use Conventional Commits for commit messages (e.g. `docs: add AGENTS.md ...`).
- Update this file when the stack, entrypoints, and commands are decided; keep it to verified facts only.
