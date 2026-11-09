# psychoResearch

Programa abierto de investigación en psicología. Recorre, con un mismo criterio, las cuatro tradiciones con que hoy se investiga en la disciplina: la **experimental**, de la que nace; la **instrumental**; la **asociativa y social**; y la **cualitativa**.

**Sitio:** https://emorito.github.io/psychoresearch/

## Qué ofrece

- **12 unidades**, de las raíces experimentales a la comunicación de resultados (ver [`docs/CURRICULO.md`](docs/CURRICULO.md)).
- **Un ciclo de estudio de nueve pasos por unidad:** ubicación en la cadena del proyecto, diagnóstico, estudio, conceptos, práctica guiada, práctica adaptativa, verificación de dominio, autoauditoría del propio proyecto y cierre.
- **Herramientas de muestreo sin pseudocálculo:** un árbol de decisión y una calculadora que primero pregunta cómo se seleccionan los casos y para qué, y solo después calcula.
- **Rutas sugeridas** para estudiantes de grado, tesistas y profesionales que investigan.

## Obras de referencia

McGuigan, *Psicología experimental* · Kerlinger y Lee, *Investigación del comportamiento* · Kazdin, *Research Design in Clinical Psychology* · *APA Handbook of Research Methods in Psychology* · APA, *JARS* · Campbell y Stanley, *Experimental and Quasi-Experimental Designs for Research* · Nunnally y Bernstein, *Psychometric Theory* · Kish, *Statistical Design for Research* · Snedecor y Cochran, *Statistical Methods*.

## Estado

En construcción. Disponibles: unidad 4 (Medición y psicometría) y unidad 8 (Muestreo e inferencia). El resto, en preparación. Ver [`ESTADO.md`](ESTADO.md).

## Uso local

```bash
python3 -m http.server 8000   # luego abrir http://localhost:8000
node --test tests/*.mjs       # pruebas de las herramientas de muestreo
```

Sitio estático (HTML, CSS y JavaScript con módulos ES), sin paso de compilación. Instrucciones para agentes en [`AGENTS.md`](AGENTS.md).

## Autor

Enrique Morosini, psicólogo.
