# Encargo para Antigravity — contenido de psychoResearch

**Lee primero `AGENTS.md` y `docs/CURRICULO.md`.** Repo local: clonar `https://github.com/emorito/psychoresearch` (rama `main`). En este repo **sí puedes hacer commits** en una rama `contenido-antigravity` (nunca en `main`); Claude revisa y fusiona.

## Tarea — Cápsulas y borradores de las unidades en preparación

Orden: u05, u06, u01, u03, u07, u09, u11, u02, u10, u12.

Para cada unidad `uNN`:

1. **Cápsula** en `data/contenido/uNN.json`, con el mismo formato que `data/contenido/u08.json`: entre 6 y 10 bloques (`table`, `cards`, `checklist`, `highlight`), terminando con un `checklist` titulado «Qué tiene que quedar reportado (APA, JARS)». Agregar `autoauditoria` (6 a 8 preguntas en primera persona sobre el propio proyecto) y `fuentes` (referencias APA completas). Poner `"origen": "borrador_ia"` en la raíz del archivo.
2. **Casos** en `casos`: tres por unidad (resuelto, a completar y libre), con el formato de `data/contenido/u08.json`.
3. **Ítems** en `data/banco/uNN.json`: 40 por unidad (12 de dificultad 1, 18 de dificultad 2 y 10 de dificultad 3), con `estado: "revisar"` y `origen: "borrador_ia"`. Distractores tomados de errores reales de estudiantes, nunca absurdos. `lectura_ref` con obra del canon y capítulo.
4. **Tarjetas**: 8 a 10 por unidad en `data/banco/flipcards.json` (`id`, `modulo_id`, `frente`, `dorso`, `tag`).
5. Cuando la unidad esté completa, cambiar `estado_contenido` a `"disponible"` en `data/modulos.json` **solo después** de la aprobación de Claude.

## Fuentes

Canon: sección 1 bis de `docs/plan-v3-y-psychoresearch.md`. En la Mac de Enrique:
- `~/Library/CloudStorage/OneDrive-Personal/Documentos/Docencia 2026/Clases UNIBE/Metodología II/Diseno de Investigacion/Archivos MD/` (Kerlinger, Kazdin, Campbell y Stanley, Shadish et al., Kish, APA Handbook en 3 volúmenes, Marradi, Brough, Ato et al.).
- `~/Library/CloudStorage/OneDrive-Personal/Estadística & Psicometría/` (Psicometría, Reliability, Sampling, N-1 single case).
- `~/Library/CloudStorage/OneDrive-Personal/Documentos/Taller TFG 2024/` (Danziger; Cumming y Calin-Jageman; Ruth, Wutich y Bernard; Ravitch y Riggan).

No descargues libros de internet. Delega en Ollama las conversiones y verificaciones mecánicas.

## Reglas de estilo

Tuteo neutro; sin voseo; sin UNIBE ni cursada. Mejor calidad que extensión: bloques breves, sin explicar lo obvio.
