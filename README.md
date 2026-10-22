# GYM LOG

Aplicación web en español para organizar rutinas de gimnasio y registrar entrenamientos. No requiere cuenta ni servidor: los datos se guardan en el almacenamiento local del navegador.

## Funciones

- Rutinas iniciales y creación, edición, duplicado, exportación e importación de rutinas.
- Registro de peso, repeticiones, series completadas, notas y descansos.
- Reanudar una sesión sin terminar, incluso después de salir de la pantalla o volver a abrir la aplicación en el mismo navegador.
- Botón **Guardar y salir** para dejar una sesión en curso y retomarla después.
- Añadir ejercicios durante una sesión y sustituir un ejercicio por otro sin perder el resto del entrenamiento. Al sustituirlo, se reinician las series de ese ejercicio para evitar mezclar registros.
- Historial y estadísticas básicas.
- Copias de seguridad JSON descargables y restaurables.
- Aviso para crear una copia local después de guardar una rutina o terminar una sesión. Permite descargarla, no recibir recordatorios durante una semana o desactivar los recordatorios para siempre.

## Publicar gratis con GitHub Pages

1. Crea un repositorio en GitHub, por ejemplo `gym-log`.
2. Sube todos los archivos y carpetas de este proyecto, incluida `.github/workflows/deploy-pages.yml`.
3. En el repositorio abre **Settings → Pages** y selecciona **GitHub Actions** como método de publicación.
4. Abre la pestaña **Actions** y espera a que termine el flujo `Deploy GYM LOG to GitHub Pages`.
5. La URL habitual será `https://TU-USUARIO.github.io/gym-log/`.

El flujo publica el contenido del repositorio en cada actualización de la rama `main`.

## Datos y copias de seguridad

Los datos se guardan en `localStorage` del navegador. No se sincronizan entre dispositivos ni se envían a GitHub. Borrar los datos del sitio, cambiar de navegador o dispositivo puede hacer que se pierdan. Descarga periódicamente la copia JSON y guárdala en un lugar seguro. No subas copias personales de la aplicación al repositorio público.

## Limitaciones conocidas

- Esta versión no tiene cuenta, sincronización en la nube ni base de datos remota.
- El archivo `manifest.webmanifest` aporta metadatos, pero esta versión no incluye un service worker; por tanto, no garantiza instalación PWA ni funcionamiento offline tras borrar la caché.
- Las copias se descargan manualmente al dispositivo; el navegador no permite escribir silenciosamente en una carpeta local sin permiso.
- Prueba la aplicación en el navegador y dispositivo de destino antes de depender de ella para guardar tus registros.

## Desarrollo local

Abre `index.html` en un navegador moderno. Para probar Pages localmente, puedes servir la carpeta con cualquier servidor estático, por ejemplo `python -m http.server 8000`.

## Licencia

MIT. Consulta `LICENSE`.
