# Cuestionario 1: Diferencia entre transición y animación

## Pregunta

¿Cuál es la diferencia principal entre una transición (`transition`) y una animación con `@keyframes`? Mencione un caso donde usaría cada una.

## Respuesta justificada

Una transición interpola propiedades entre el valor anterior y el nuevo cuando cambia el estado del elemento, por ejemplo al activar `:hover` o `:focus`. Es adecuada para que el color de un botón cambie suavemente al pasar el cursor.

Una animación define una secuencia mediante `@keyframes`, puede contener estados intermedios y puede iniciarse al cargar la página, repetirse o alternar sin interacción. Es adecuada para un spinner que gira continuamente.

La diferencia principal es el modo de definir y activar el cambio: una transición responde a un cambio de valores; una animación sigue una secuencia de fotogramas con su propia temporización.
