# ESTADO — psychoResearch

**08/11/2026 · Arranque (Claude).**

- Motor v3 traído de meto2psico25 (`rediseno-2026`, commit 596df79): página de unidad con ciclo de 9 pasos, árbol de muestreo y calculadora honesta. Clave de almacenamiento propia (`psychoresearch.v1`).
- Página de inicio propia: tesis curricular, cuatro tradiciones, 12 unidades agrupadas, rutas por perfil y obras de referencia.
- Contenido disponible: **u08 Muestreo e inferencia** (desde m08) y **u04 Medición y psicometría** (desde m09), pasados a tuteo, con sus ítems aprobados (40 y 16) y flipcards.
- Las otras 10 unidades tienen propósito, resultados y fuentes, y una cápsula «En preparación».
- Verificación: 9 pruebas de muestreo pasan; inicio y unidades sin errores de consola ni desplazamiento horizontal a 375 y 1280 px.

**08/11/2026 · Avance u05 (Antigravity).**

- **u05 Diseño experimental y cuasiexperimental**:
  - Cápsula completa en `data/contenido/u05.json` (10 bloques: principio MAX-MIN-CON, triángulo de Kish, notación X-O-R de Campbell y Stanley, diseños preexperimentales, cuasiexperimentales y experimentales verdaderos, auditoría de amenazas a la validez interna, tensión Kish vs. Campbell & Stanley vs. Marradi, y lista de cotejo JARS).
  - Casos en `data/contenido/u05.json`: 3 minicasos analizados (X O, autoselección voluntaria en grupos no equivalentes y regresión estadística a la media) más simulación interactiva de 3 pasos.
  - Banco de ítems en `data/banco/u05.json`: 40 ítems (12 D1, 18 D2, 10 D3) con distractores basados en confusiones reales de estudiantes, referencias exactas al canon (Campbell y Stanley, Shadish et al., Kish, Kerlinger y Lee, Marradi, JARS), en estado `revisar` y origen `borrador_ia`.
  - Flipcards: 10 tarjetas en `data/banco/flipcards.json` para repaso activo.
  - Registro de subtemas y autoauditoría integrados en `data/modulos.json` (`estado_contenido` se mantiene `en_preparacion` a la espera de la aprobación de Claude).
  - Verificación: validación de esquema JSON y suite de pruebas pasando.

## Pendiente

1. Redacción de u06 (caso único, Kazdin) y detención para la revisión de Claude de u05 y u06.
2. Redacción de las 8 unidades restantes tras revisión.
3. Repaso, simulacro, progreso y glosario: llegan cuando estén terminados en meto2psico25.
4. Ítems de u04 heredados de m09: revisar que no aludan a la cursada de UNIBE.
