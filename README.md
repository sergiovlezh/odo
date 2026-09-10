# Odo - Diario del vehículo

Odo es tu bitácora del vehículo: consumo de combustible/electricidad, gastos, estaciones, diario, tareas y recordatorios.

Sin backend, sin cuentas, sin notificaciones.

Tus datos viven en tu navegador (`localStorage`); la exportación/importación en JSON es tu copia de seguridad.

> Estado: especificación inicial, sin implementación todavía. Lo descrito abajo es el objetivo, no lo existente.

Tipos soportados: `fuel` y `electric`. Los híbridos (MHEV, HEV, PHEV, REEV) quedan fuera del alcance por ahora.

## Stack

React + Vite + Tailwind + TypeScript + BrowserRouter, desplegado en Vercel.

Se requiere el rewrite SPA en `vercel.json` (`/(.*)` -> `/index.html`).

## Uso

```bash
pnpm install
pnpm dev        # http://localhost:5173
pnpm check      # jiti src/domain.selfcheck.ts
pnpm build      # tsc -b && vite build -> dist/
pnpm lint       # oxlint
```

Verificación antes de cada commit:
`pnpm check && pnpm build && pnpm lint`

## Ramas
- main = producción. Protegida.
- dev = integración. Protegida.
- Una rama por tarea desde dev: feat/…, fix/…, refactor/…, chore/….
- PR con plantilla hacia dev. Release con PR dev -> main.

## Licencia
MIT © Sergio V - ver [LICENSE](LICENSE).

## For Contributors
- Code and PRs in English.
- User strings ship in ES in the same commit as the UI that uses them.
- The t() skeleton and Lang type stay so contributors can add EN later; EN values may go stale. No dead ES keys.
