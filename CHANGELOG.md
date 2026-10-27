# Changelog

## 1.04
- Actualización visual a negro, rojo y amarillo.
- Nuevo logotipo en la cabecera y nuevo favicon.
- Mejoras de legibilidad, jerarquía visual, controles y navegación adaptable.
- Sin cambios intencionados en la funcionalidad.

Historial de cambios

## Versión 1.03

- Renombrado el botón superior **Compartir enlace** a **Compartir GYM LOG**.
- Eliminado el botón **Exportar** de cada tarjeta de rutina para evitar duplicidad; se mantiene **Compartir rutina**, que comparte la rutina individual y descarga el archivo si no hay una función nativa de compartir disponible.
- Actualizado el indicador de versión visible a `v1.03`.

# Historial de cambios

## Versión 1.02

- Añadido un paso previo a la importación desde texto para indicar el nombre de la rutina y el número de días de entrenamiento.
- Mejorada la detección y asignación de ejercicios por encabezados; cuando no hay encabezados, los ejercicios se reparten entre los días elegidos.
- La vista previa permite editar el nombre de cada día, mover ejercicios entre días, cambiar series/repeticiones y eliminar ejercicios antes de guardar.
- Añadida la opción **Compartir rutina** para compartir/exportar una sola rutina sin enviar las demás ni el historial.
- Añadido el botón **Compartir enlace**, que copia la URL de la aplicación.
- Añadida la etiqueta de versión discreta en una esquina de la interfaz.

## Versión 1.01

- Añadido **Guardar y salir** para dejar una sesión activa y retomarla más tarde.
- Corregido el botón **Añadir ejercicio** durante un entrenamiento.
- Añadida la opción **Cambiar** para sustituir un ejercicio durante la sesión.
- Las rutinas guardadas pueden editarse desde la pantalla de Rutinas.
- Añadido un recordatorio de copia de seguridad tras guardar una rutina o terminar una sesión, con opciones de recordatorio semanal o desactivación permanente.

## Versión inicial

- Rutinas, registro de series, temporizador, historial, estadísticas y copias JSON.
### Corrección de enlace para compartir (v1.03)
- El botón «Compartir GYM LOG» utiliza ahora la URL pública fija `https://jmrb92.github.io/GYMLOG/?utm_source=chatgpt.com`.
- Copia el enlace al portapapeles y muestra confirmación; si el navegador bloquea la copia, ofrece un cuadro de texto para copiarlo manualmente.

### Corrección de mantenimiento (sin cambio de versión: v1.03)
- El botón «Compartir GYM LOG» abre ahora un diálogo visible con el enlace exacto, copiar con alternativa manual y compartir mediante el menú nativo cuando está disponible.
