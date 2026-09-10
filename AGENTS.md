# AGENTS.md

Spec-first repo, no code on any branch. `README.md` (ES) is the spec: vehicle journal ("bitácora del vehículo"), localStorage-only, no backend; target stack React + Vite + Tailwind + TS on Vercel; branches main/dev + PR template.

- Target commands per README (unverified, no code yet): `npm run dev|check|build|lint`; pre-commit gate `npm run check && npm run build && npm run lint`. Do not invent others.
- Keep docs/UX copy in Spanish unless asked otherwise (README is Spanish); code and PRs in English. User strings ship in ES in the same commit as the UI that uses them; keep the t() skeleton and Lang type for future EN, no dead ES keys.
- Use Conventional Commits for commit messages (e.g. `docs: add AGENTS.md ...`).
- Update this file when the stack, entrypoints, and commands are decided; keep it to verified facts only.
