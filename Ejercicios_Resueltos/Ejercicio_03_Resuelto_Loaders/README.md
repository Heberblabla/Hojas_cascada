# Resuelto 3: Spinner y barra de progreso

Origen: páginas 6-8 de la guía, en el orden del documento.

## Solicitud

Crear un spinner de giro continuo y una barra que alterne llenado y vaciado.

## Solución

Se reproduce el diseño de la guía: spinner cian sobre fondo oscuro y barra de 300 px. `linear` mantiene uniforme la rotación; `alternate` invierte la barra en cada ciclo y `scaleX` evita animar su ancho.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

1. El spinner completa una vuelta cada segundo.
2. La barra se llena en 2.5 s y se vacía en los siguientes 2.5 s.
3. Cambia temporalmente `linear` por `ease` en `.spinner` y compara.
4. Abre F12 → More tools → Animations y reduce la velocidad al 10 % para observar los fotogramas.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.

## Resultado de la comparación solicitada

Con `ease`, el giro acelera y frena en cada vuelta; con `linear` la velocidad angular es constante. La barra mantiene su anclaje izquierdo al invertir la dirección. Es una demostración de carga, sin una descarga real ni un porcentaje de datos asociado.
