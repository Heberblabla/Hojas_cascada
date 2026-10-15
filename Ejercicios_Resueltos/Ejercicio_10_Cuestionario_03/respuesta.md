# Cuestionario 3: Curva de aceleración y repeticiones

## Pregunta

Explique qué hacen `animation-timing-function` y `animation-iteration-count`. Indique dos valores posibles para cada una.

## Respuesta justificada

`animation-timing-function` determina cómo progresa la interpolación en el tiempo entre fotogramas. Dos valores son:

- `linear`: avance uniforme; apropiado para un giro continuo.
- `ease-in-out`: suaviza el inicio y el final de cada tramo.

`animation-iteration-count` determina cuántos ciclos se reproducen. Dos valores son:

- `3`: ejecuta tres ciclos y termina.
- `infinite`: repite indefinidamente.

Ejemplo: `animation: girar 1s linear infinite` da al spinner un ciclo de un segundo, progreso uniforme y repetición sin límite. La duración de un ciclo y la cantidad de ciclos son propiedades diferentes.
