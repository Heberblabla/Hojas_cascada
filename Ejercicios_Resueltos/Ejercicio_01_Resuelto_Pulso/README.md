# Resuelto 1: Botón con efecto de pulso

Origen: páginas 3-4 de la guía, en el orden del documento.

## Solicitud

Crear un botón con pulso infinito y pausarlo al pasar el cursor.

## Solución

Se reproducen el botón azul, el fondo oscuro y los fotogramas de la guía. `transform` cambia la escala y `box-shadow` crea el halo; `animation-play-state` conserva el instante al pausar.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

1. Observa el crecimiento y el halo cada 1.5 s.
2. Pasa el cursor: se detiene; retíralo: continúa. También se pausa al enfocarlo con Tab.
3. Para la comparación del paso 3, cambia temporalmente `1.5s ease-in-out` por `0.6s linear` en CSS y recarga. Restaura los valores al terminar.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.

## Resultado de la comparación solicitada

Con 0.6 s el ciclo se repite 2.5 veces más rápido. `linear` interpola uniformemente entre fotogramas; `ease-in-out` suaviza el comienzo y el final de cada tramo. La velocidad global todavía depende de los valores y porcentajes de los fotogramas.

Suposición: el botón es una demostración visual; el PDF no pide un formulario ni una acción de inscripción.
