# Propuesto 1: Logo con rebote

Origen: páginas 8 de la guía, en el orden del documento.

## Solicitud

Círculo o ícono con rebote infinito, tres porcentajes, `ease-in-out`, `alternate` y sombra que se reduzca al subir.

## Solución

Un círculo CSS usa fotogramas 0 %, 50 % y 100 %. La sombra tiene los mismos tiempos, dirección y repeticiones; su escala y opacidad bajan cuando el círculo está arriba.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

Observa varios ciclos: el círculo sube 100 px y vuelve al suelo; la sombra se reduce al 45 % de su ancho en el punto más alto. Inspecciona `animation-direction: alternate` y `animation-timing-function: ease-in-out` en F12.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.

Suposición: se elige el círculo permitido por el enunciado; las letras CSS son decoración, no un logo institucional.
