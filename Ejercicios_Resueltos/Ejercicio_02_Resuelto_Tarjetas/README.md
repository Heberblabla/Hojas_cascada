# Resuelto 2: Tarjetas con entrada escalonada

Origen: páginas 5-6 de la guía, en el orden del documento.

## Solicitud

Tres tarjetas deben aparecer con desvanecimiento y desplazamiento hacia arriba, en secuencia y conservando el estado final.

## Solución

Se mantienen los contenidos, colores, duración y retardos del ejemplo. Solo se animan `opacity` y `transform`. La cuadrícula se adapta a pantallas pequeñas.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

1. Recarga con Ctrl + F5: comienzan a los 0.2, 0.5 y 0.8 s.
2. Al finalizar, las tres tarjetas permanecen visibles.
3. Quita temporalmente `forwards` y recarga; después prueba `cubic-bezier(.68,-0.55,.27,1.55)` en lugar de `ease-out`. Restaura el CSS tras comparar.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.

## Resultado de las comparaciones solicitadas

Sin `forwards`, al terminar cada animación vuelve el estilo base `opacity: 0`, por lo que la tarjeta desaparece. La curva `cubic-bezier(.68,-0.55,.27,1.55)` produce anticipación y sobrepaso en la traslación; la opacidad se limita a su rango válido. `ease-out` desacelera la llegada sin ese efecto elástico.
