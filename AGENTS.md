# AGENTS.md — psychoResearch

Programa abierto de investigación en psicología, sin adscripción institucional. Nace del rediseño v3 de meto2psico25 y comparte su motor (`assets/js/engine.js`, `modulo-app.js`, `store.js`, `muestreo/`).
Dirección y revisión: Claude. Decisión final: Enrique Morosini.

## Documentos que mandan

1. `docs/plan-v3-y-psychoresearch.md`: canon de autoridad (sección 1 bis), principio antipseudocálculo (sección 1), currículo (sección 3).
2. `docs/CURRICULO.md`: las 12 unidades, sus propósitos, resultados y fuentes.
3. Tu encargo: `docs/ENCARGO-ANTIGRAVITY.md` (contenido) o `docs/ENCARGO-CODEX.md` (código, cuando exista).
4. `REVISION.md`: observaciones de Claude que se aplican antes de seguir.

## Reglas fijas

- **Registro: castellano neutro con tuteo.** Nunca voseo («revisa», no «revisá»; «puedes», no «podés»). Sin referencias a UNIBE, a clases, fechas de cursada ni Moodle.
- **Canon:** todo contenido se ancla en las obras de la sección 1 bis del plan. Si dos discrepan, se muestra la tensión.
- **Muestreo:** nunca margen de error ni nivel de confianza con muestras no probabilísticas; nunca tamaño de muestra calculado para un estudio cualitativo.
- **El contenido existente no se reescribe:** lo dudoso se marca `estado: "revisar"` con `nota_revision`.
- **Contenido nuevo** entra con `origen: "borrador_ia"` y `estado: "revisar"`; el sitio solo muestra ítems `aprobado`.
- **No se publican** protocolos ni ítems de tests comerciales.
- **Sin compilación:** HTML, CSS y JS con módulos ES; funciona tal cual en GitHub Pages.
- **Motor compartido:** los cambios de motor se hacen primero en meto2psico25 (rama `rediseno-2026`) y se traen aquí; no se bifurca el motor sin acuerdo.
- Al cerrar cada tarea, actualizar `ESTADO.md`.

## Estructura de datos

- `data/modulos.json`: 12 unidades (`u01`–`u12`) con `eslabon_cadena`, `fuentes_canon` y `estado_contenido` (`disponible` / `en_preparacion`).
- `data/contenido/uNN.json`: cápsula (bloques `table`, `cards`, `checklist`, `highlight`, `herramienta`), `casos`, `recursos`, `autoauditoria`.
- `data/banco/uNN.json`: `{ "modulo_id": "uNN", "items": [...] }`, mismo esquema que meto2psico25.
- `data/banco/flipcards.json`: tarjetas con `modulo_id`.

## Verificación

```bash
python3 -m http.server 8000
node --test tests/*.mjs
```
