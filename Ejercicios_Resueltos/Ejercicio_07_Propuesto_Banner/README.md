# Propuesto 4: Banner con fondo animado

Origen: páginas 8 de la guía, en el orden del documento.

## Solicitud

Banner de bienvenida con degradado móvil, `background-size: 400% 400%`, animación de `background-position`, título con fade-in y desactivación mediante `prefers-reduced-motion`; comentar propiedades.

## Solución

El fondo alterna su posición durante 10 s por ciclo. El título aparece una sola vez con opacidad de 0 a 1. Los comentarios CSS desglosan cada atajo de animación. Se conserva el movimiento del fondo solicitado aunque requiere repintado.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

1. Recarga y observa el fade-in del título y el desplazamiento del degradado.
2. En F12 → More tools → Rendering emula `prefers-reduced-motion: reduce` (o activa reducir movimiento en el sistema).
3. Deben detenerse fondo y título; el título sigue visible. Restaura `no-preference` para recuperar las animaciones.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.


