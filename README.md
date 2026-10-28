# GYM LOG Web · v1.08 revisada

Aplicación web de entrenamiento en español. Mantiene el diseño negro, rojo y amarillo y las funciones de registro de rutinas y entrenamientos. No requiere cuenta ni servidor de datos: la información personal se guarda en el almacenamiento local del navegador.

## Funciones conservadas

- Rutinas de serie: **Full Body de 2 días**, **Push Pull Legs de 3 días**, **Hipertrofia de 5 días** y **Rutina híbrida de 5 días**. Se muestran siempre en «Mis rutinas», no se pueden editar ni eliminar y se pueden duplicar.
- Rutinas propias: creación desde cero, edición, duplicado, activación/desactivación, eliminación e importación desde texto o archivo.
- Inicio: muestra únicamente las rutinas activas y el calendario de actividad de las últimas 12 semanas. La semana actual queda al final del área desplazable; los días empiezan en lunes, los meses aparecen en vertical y los entrenamientos finalizados se marcan en verde.
- Registro de entrenamientos: series, peso, repeticiones/tiempo, notas, descansos, añadir/quitar ejercicios y series, sustituir ejercicios y guardar/reanudar una sesión.
- Biblioteca de ejercicios: búsqueda, filtro por grupo y creación/edición de ejercicios personalizados.
- Historial, detalle de sesiones y progreso de cargas.
- Temporizador de descanso configurable y opción de inicio automático.
- Copia de seguridad completa JSON, restauración, exportación de rutinas y compartir una sola rutina mediante archivo `.gymlog`.
- Botón «Compartir GYM LOG» con la URL pública exacta: https://jmrb92.github.io/GYMLOG/.

## Publicar en GitHub Pages

1. Descomprime este ZIP.
2. Sube **el contenido de esta carpeta directamente a la raíz** del repositorio `JMRB92/GYMLOG`, de modo que `index.html` quede en la raíz junto a `gym-log-logo.png`.
3. Si el repositorio ya publica GitHub Pages, espera a que termine la publicación y abre https://jmrb92.github.io/GYMLOG/.
4. Si necesitas configurar Pages, entra en **Settings → Pages** y configura el origen correspondiente al repositorio. El flujo incluido en `.github/workflows/deploy-pages.yml` publica la rama `main` mediante GitHub Actions.

No subas archivos de copia de seguridad personales al repositorio público.

## Datos y privacidad

Los datos se guardan en `localStorage` del navegador. No hay cuenta ni sincronización entre dispositivos y la aplicación no envía las rutinas o el historial a un servidor propio. Borrar los datos del sitio, cambiar de navegador o dispositivo puede hacer que se pierdan. Descarga periódicamente una copia JSON y guárdala en un lugar seguro.

El manifiesto contiene metadatos de instalación, pero esta versión no incorpora un service worker; por tanto, no garantiza uso sin conexión ni funcionamiento en segundo plano tras cerrar el navegador.

## Prueba local

- Para probar todas las funciones, abre `index.html` desde un servidor estático (por ejemplo, `python -m http.server 8000`) y visita `http://localhost:8000`.
- Se incluye además un archivo HTML independiente en la entrega, con el logotipo incrustado, para abrirlo directamente en el navegador. Sus datos se guardan por separado de los de la URL publicada.

## Historial de cambios

### v1.08 revisada
- Conserva la interfaz y las funciones web existentes.
- Corrige el enlace de compartir para usar la URL pública exacta.
- Corrige la creación de ejercicios personalizados desde el selector de ejercicios del editor de rutinas, sin perder el editor abierto.
- Recupera las rutinas de serie que falten al cargar datos antiguos o restaurar copias, sin sobrescribir las rutinas del usuario.
- Evita reactivar automáticamente una rutina si el usuario ha desactivado intencionadamente todas las rutinas.
- Refuerza la importación de rutinas y la normalización de datos.
