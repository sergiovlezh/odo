# Política de seguridad / Security Policy

## Español

### Versiones soportadas

Solo `main` tiene soporte. `dev` y ramas `feat/*` no.

### Cómo reportar

NO abras un issue público. Usa la pestaña **Security > Report a vulnerability**
(reporte privado). Incluye: URL/commit afectado, pasos para reproducir, impacto.

Responsable: @sergiovlezh. Respuesta por mejor esfuerzo, sin SLA fijo.

### Alcance

Frontend-only, sin backend. Riesgos realistas: XSS vía notas/import,
JSON de respaldo malicioso. Los datos de `localStorage` nunca salen del
navegador salvo exportación iniciada por el usuario.

## English

### Supported versions

Only `main` is supported. `dev` and `feat/*` branches are not.

### How to report

Do NOT open a public issue. Use **Security > Report a vulnerability**
(private report). Include: affected URL/commit, reproduction steps, impact.

Maintainer: @sergiovlezh. Best-effort response, no fixed SLA.

### Scope

Frontend-only, no backend. Realistic risks: XSS via notes/import,
malicious backup JSON. `localStorage` data never leaves the browser
except via user-initiated export.
