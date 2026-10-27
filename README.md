# GYM LOG · versión 1.03

Aplicación web en español para organizar rutinas de gimnasio y registrar entrenamientos. No requiere cuenta ni servidor: los datos se guardan en el almacenamiento local del navegador.

## Funciones

- Rutinas iniciales y creación, edición, duplicado e importación de rutinas.
- Importación desde texto con nombre y número de días definidos antes de analizar; vista previa para mover ejercicios de un día a otro y ajustar nombres de días.
- Compartir una sola rutina en un archivo `.gymlog`, sin incluir el resto de las rutinas ni el historial.
- Botón **Compartir GYM LOG** para copiar la URL de la aplicación y enviársela a otra persona.
- Número de versión visible discretamente en una esquina de la interfaz.
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


**Compartir GYM LOG:** el botón superior abre un diálogo con el enlace público `https://jmrb92.github.io/GYMLOG/?utm_source=chatgpt.com`. Si el navegador bloquea el portapapeles, permite seleccionar y copiar el enlace manualmente.


## Versión 1.04 — identidad visual
- Nueva identidad visual negro, rojo y amarillo.
- Logotipo actualizado con el diseño proporcionado.
- Tipografía, contraste, botones, navegación y tarjetas ajustados para facilitar la lectura.
- Sin cambios intencionados en la lógica ni en las funciones de la aplicación.
