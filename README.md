# tecweb-tp-skill

Skill para [opencode](https://opencode.ai) que ayuda a los alumnos de **Tecnologías Web**
(TUARI/UNICEN) a hacer el TP de la materia (backend NestJS + frontend Angular) con IA, sin que
la IA se lo resuelva de una. Fuerza que el alumno explique lo que va entendiendo, avanza paso a
paso, genera diagramas entidad-relación, chequea contra la consigna real, y explica los
conceptos con la misma terminología y ejemplos que se dieron en clase (no de forma genérica).

## Cómo instalarla en el repo del TP

Copiá estos dos elementos a la raíz del repo del TP:

- `AGENTS.md`
- `.opencode/`

opencode los detecta solos: `AGENTS.md` se carga siempre y le dice al agente que consulte la
skill; la skill (`tp-tecnologias-web`) se activa cuando el trabajo tiene que ver con el proyecto.
No hace falta ningún paso de instalación adicional.

## Estructura

```
AGENTS.md                                        # instrucciones siempre cargadas: "consultá la skill"
.opencode/skills/tp-tecnologias-web/
├── SKILL.md                                      # reglas pedagógicas + resumen de la consigna
└── references/
    ├── nestjs-catedra.md                         # conceptos de las 8 clases de NestJS de la cátedra
    ├── angular-catedra.md                        # conceptos de las 7 clases de Angular de la cátedra
    ├── rest-mvc-catedra.md                        # conceptos de las teóricas de REST y MVC
    ├── docs-oficiales.md                          # links a la documentación oficial de NestJS/Angular
    └── videos-catedra.md                          # índice de las 22 clases grabadas en YouTube (link + timestamps)
```

## Qué hace la skill (resumen)

- No asume decisiones de diseño por el alumno (entidades, campos) — pregunta y ofrece opciones.
- Da pistas antes que código; nunca resuelve el TP de una si se lo piden directamente.
- Avanza en pasos chicos con checkpoints de comprensión — pide que el alumno explique el código
  antes de seguir.
- Explica los conceptos anclados al material real de la cátedra (mismo ejemplo "Brewery" usado
  en clase, misma terminología) en vez de explicaciones genéricas de NestJS/Angular.
- Genera un diagrama entidad-relación apenas se define el modelo de datos.
- Al cerrar cada entrega, chequea explícitamente contra los requisitos obligatorios de la
  consigna.
- Le recuerda al alumno guardar el historial de la conversación, porque se entrega junto con el
  TP como evidencia del proceso.
- Reconoce patrones repetidos (ej. la segunda entidad del CRUD) para no ser redundante y no
  volverse tedioso.

## Origen del contenido

Las reglas pedagógicas se armaron y probaron con simulaciones de alumnos (uno apurado pidiendo
"hacé todo de una", otro cooperativo) antes de esta versión. El contenido de `references/` se
extrajo de las slides reales de la cátedra (carpeta de Drive de la materia), de la
documentación oficial de NestJS y Angular, y de las 22 clases grabadas en el canal de YouTube de
la cátedra (`videos-catedra.md`), procesadas a partir de su transcript/subtítulos completo (21
vía el editor de YouTube Studio del canal, 1 vía el panel público de YouTube). Solo uno de los 22
videos tiene timestamps exactos por segmento; el resto tiene timestamps aproximados, estimados
proporcionalmente a partir del orden de los temas en el transcript (marcado así en cada entrada).
Vale la pena que un docente los revise antes de darlos por definitivos.

## Mantenimiento

Si cambia la consigna del TP, actualizá la sección "La consigna (resumen)" en `SKILL.md`. Si se
actualizan las slides de la cátedra, volvé a generar los archivos de `references/` a partir del
material nuevo.
