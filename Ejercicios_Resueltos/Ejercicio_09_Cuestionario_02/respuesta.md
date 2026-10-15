# Cuestionario 2: Regla @keyframes y fotogramas

## Pregunta

¿Para qué sirve la regla `@keyframes` y qué diferencia hay entre definir sus pasos con `from/to` y hacerlo con porcentajes?

## Respuesta justificada

`@keyframes` define los valores de las propiedades en determinados instantes de una animación con nombre. Se aplica a un elemento mediante `animation-name` o el atajo `animation`.

`from` equivale a `0%` y `to` equivale a `100%`: describen los extremos. Los porcentajes permiten añadir pasos intermedios, por ejemplo `0%` en el suelo, `50%` arriba y `100%` nuevamente en el suelo. El navegador interpola entre esos valores.

Si solo hay dos estados, `from/to` y `0%/100%` son equivalentes. Usar porcentajes no obliga a tener más pasos, pero permite expresarlos con precisión.
