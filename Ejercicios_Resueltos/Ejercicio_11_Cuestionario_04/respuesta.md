# Cuestionario 4: Persistencia con forwards

## Pregunta

¿Qué efecto tiene `animation-fill-mode: forwards` y por qué es útil en animaciones de entrada?

## Respuesta justificada

`forwards` mantiene los valores animados del último fotograma reproducido cuando finaliza la animación. Es útil para que una tarjeta que entra con opacidad de 0 a 1 y desplazamiento de 40 px a 0 permanezca visible y en su posición final.

En el ejercicio resuelto 2, sin `forwards` vuelve a aplicarse la opacidad base `0` y la tarjeta desaparece. Con `forwards` conserva la opacidad `1` del final.

No modifica permanentemente la hoja de estilos ni conserva necesariamente el fotograma escrito como `100%`: el último fotograma reproducido depende de la dirección y de las iteraciones. Para una entrada normal de una iteración sí corresponde a `100%`. `forwards` tampoco aplica el primer fotograma durante el retardo; para eso se usa `backwards` o `both`.
