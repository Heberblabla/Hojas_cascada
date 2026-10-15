# Propuesto 3: Tres puntos de carga

Origen: páginas 8 de la guía, en el orden del documento.

## Solicitud

Tres puntos centrados que aumentan y disminuyen su tamaño en secuencia, con un solo `@keyframes`, tres retardos y repetición infinita.

## Solución

Los tres círculos reutilizan `ola`, con retardos 0, .2 y .4 s. `scale` modifica el tamaño sin alterar el espacio de la fila. Grid centra el conjunto en ambos ejes.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

Observa varias ondas: el primer punto crece antes que el segundo y el tercero. En F12 verifica que los tres comparten `animation-name: ola`, tienen retardos distintos e iteración infinita.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.


