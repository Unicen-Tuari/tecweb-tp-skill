# Changelog — tp-tecnologias-web

Este archivo lleva el registro de versiones de la skill, para que el chequeo automático de
actualizaciones (ver `AGENTS.md`) le pueda mostrar al alumno qué cambió antes de actualizar.

Al publicar una versión nueva: subí el número en
`.opencode/skills/tp-tecnologias-web/VERSION` (formato `MAJOR.MINOR.PATH`, sin la `v`) y agregá
una entrada acá arriba de todo.

## 1.1.0 — 2026-10-21

Ajustes a partir de revisar los primeros TPs entregados (Entrega 1) y sus logs de sesión, más
lo que conviene tener previsto para la Entrega 2 (Angular + deploy):

- Antes del primer commit se verifica el `.gitignore` (`nest new --skip-git` no lo crea y
  `node_modules/` terminaba en el repo).
- El chequeo final de la primera entrega ahora incluye que el repo sea reproducible: README
  propio, `.env.example`, `docker-compose.yml`, nada de `node_modules`/`dist`/datos de la base
  en el repo, y filtros inválidos que respondan 400.
- Checkpoints más estrictos: no se valida una respuesta con el porqué equivocado, y después de
  corregir se pide que el alumno lo reformule antes de avanzar.
- La primera vez que aparece cada pieza nueva, el intento del alumno tiene que ser código suyo,
  no solo una descripción.
- La colección de Postman deja de tratarse como paso operativo: el alumno arma al menos una parte.
- Nueva sección "Frontend y deploy: lo que suele fallar": URL de la API por `environments`,
  publish dir y `_redirects` en Netlify, `PORT`/CORS/servicio dormido/vencimiento del Postgres
  gratis en Render, formularios template-driven, errores del backend en la UI, el `<select>` de
  la relación y checkpoints propios de Angular.
- El chequeo final de la segunda entrega verifica los deploys (incógnito, refresh en ruta
  interna, nada de `localhost` en el build, errores visibles en la UI).
- La nota de versión de Angular suma los cambios de v15 (`environments`), v18 (`public/`) y v20
  (nombres de archivo sin sufijo).

## 1.0.0 — 2026-08-28

Primera versión con versionado formal. Incluye todo el trabajo hecho hasta acá:

- Reglas pedagógicas completas (no asumir, pistas antes que código, pasos chicos con checkpoint,
  diagrama entidad-relación, chequeo contra la consigna, reconocer patrones repetidos).
- Regla de control de versiones: backend y frontend en dos repos de GitHub separados, y recordar
  commitear al cerrar cada parte funcional.
- Referencias de cátedra: NestJS (8 clases), Angular (7 clases), REST/MVC (teóricas), links a
  documentación oficial de NestJS y Angular.
- Índice de las 22 clases grabadas en YouTube, todas procesadas con transcript/subtítulos
  completo.
- Chequeo automático de actualizaciones al arrancar una sesión nueva (este mismo mecanismo).
