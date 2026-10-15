# Cuestionario 5: Rendimiento y movimiento reducido

## Pregunta

¿Por qué se recomienda animar `transform` y `opacity` en lugar de `width`, `height` o `top`? ¿Qué es `prefers-reduced-motion` y para qué se utiliza?

## Respuesta justificada

`transform` cambia la representación visual del elemento y `opacity` su transparencia sin modificar normalmente el espacio que ocupa en el flujo. El navegador suele poder procesarlas en la fase de composición, evitando recalcular el diseño en cada fotograma.

Animar `width` o `height` altera dimensiones y puede obligar a recalcular la distribución y repintar. Animar `top` cambia la posición de un elemento posicionado y también puede requerir trabajo de diseño o pintura. Por eso se prefiere `translate` para desplazar y `scale` para cambiar el tamaño visual. La mejora concreta depende del navegador y del contenido; no se garantiza aceleración GPU en todos los casos.

`prefers-reduced-motion` es una característica de las media queries que consulta la preferencia del usuario por reducir el movimiento, normalmente configurada en el sistema operativo. No detecta una enfermedad: permite adaptar la interfaz para evitar movimiento innecesario o molesto.

Ejemplo aplicado al banner:

```css
@media (prefers-reduced-motion: reduce) {
  .banner, h1 { animation: none; }
  h1 { opacity: 1; }
}
```

Se detiene el fondo y se conserva el título visible. Desactivar una animación de entrada sin restaurar una opacidad base oculta podría hacer desaparecer el contenido.
