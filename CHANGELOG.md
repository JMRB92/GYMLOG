# Historial de cambios GYM LOG Web

## v1.08 revisada
- Conserva las funciones de la versión web existente.
- Las rutinas de serie están protegidas, siempre se muestran en «Mis rutinas» y pueden duplicarse, pero no editarse ni eliminarse.
- Las rutinas propias se pueden crear, editar, duplicar, activar/desactivar y eliminar.
- Inicio muestra solo las rutinas activas y el calendario semanal de actividad.
- Calendario de 12 semanas, lunes a domingo, continuidad entre meses, meses en vertical y semana actual al final del área desplazable.
- Enlace «Compartir GYM LOG» corregido a `https://jmrb92.github.io/GYMLOG/`.
- Selector de ejercicios personalizado corregido para que crear un ejercicio dentro del editor de rutinas no cierre ni destruya el editor.
- Migración de datos antiguos: se recuperan rutinas de serie ausentes y se conservan las rutinas propias.
- Restauración e importación de rutinas reforzadas para mapear los ejercicios importados con la biblioteca local.
- Se evita reactivar automáticamente una rutina cuando el usuario ha desactivado intencionadamente todas.
- Se incluyen el manifiesto, el favicon y el flujo de publicación de GitHub Pages que faltaban en el paquete anterior.
