# Historial de cambios GYM LOG Web

## v1.09 revisada
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

## v1.09
- En móvil, el lema del encabezado aparece debajo del logotipo y los botones, ocupando todo el ancho.
- La edición de cada ejercicio de una rutina se abre en una ventana independiente con series, repeticiones, descanso, variante y notas.
- Progreso reorganizado: muestra primero peso y repeticiones del último registro y permite abrir gráficas de valores reales y una estimación orientativa.
- Calendario con etiquetas «Realizado» y «No realizado»; al pulsar un día abre el entrenamiento correspondiente del historial.
- Se mantienen el enlace para compartir la aplicación y las funciones existentes.


### v1.09 — corrección de funcionamiento
- Alineado a la izquierda el lema del encabezado móvil.
- Reforzado el guardado de rutinas con validación visible, manejo de errores y botones explícitos de tipo button.
- Añadida validación para impedir que un identificador de rutina inexistente rompa el inicio de un entrenamiento.


### v1.09 · revisión de guardado y rutinas
- Los botones «＋ Nueva» e «Importar desde texto» aparecen juntos y permanecen accesibles al desplazarse por «Mis rutinas».
- Al guardar una rutina nueva, se abre directamente la selección de día para empezar a entrenar sin pasos confusos.
- El inicio de sesión valida la rutina y el día, admite días todavía vacíos y conserva la sesión anterior si no puede guardar.
- «Guardar y salir» y «Finalizar» comprueban el resultado del guardado; si falla el almacenamiento, la sesión no se elimina de memoria.
- El encabezado conserva el logotipo, los botones y el lema alineado a la izquierda dentro del mismo bloque fijo.
