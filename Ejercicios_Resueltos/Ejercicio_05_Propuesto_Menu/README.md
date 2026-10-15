# Propuesto 2: Menú con efecto de entrada

Origen: páginas 8 de la guía, en el orden del documento.

## Solicitud

Barra con cinco enlaces, entrada desde la izquierda con retardos crecientes, posición final persistente y transición de color al pasar el cursor.

## Solución

Cinco enlaces internos funcionales comparten `entrar`; los retardos crecen de .1 a .7 s. `both` aplica los estilos iniciales durante la espera y mantiene los finales. `transition` suaviza el color al interactuar.

## Ejecución y comprobación

Extrae el ZIP completo y abre `index.html` con doble clic en Chrome, Edge o Firefox. También puedes usar Live Server en VS Code. No requiere conexión a Internet.

1. Recarga: aparecen Inicio, Servicios, Proyectos, Nosotros y Contacto, en ese orden.
2. Al finalizar siguen visibles y sin desplazamiento.
3. Pasa el cursor o usa Tab para observar el color.
4. Pulsa cada enlace para ir a su sección.

## Dependencias

Solo un navegador moderno. Sin Node.js, JavaScript, bibliotecas, fuentes remotas ni compilación.

Suposición: el PDF permite personalizar contenido; se usan secciones internas para que los cinco enlaces tengan destino real sin servicios externos.
