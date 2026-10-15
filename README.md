# GYM LOG

Aplicación web local para registrar entrenamientos. No requiere cuentas ni servidor y guarda datos en IndexedDB del navegador.

## Ejecutar localmente
1. Descomprime la carpeta `gymlog`.
2. Para probarla, abre `index.html` en un navegador moderno. Para un comportamiento más fiable de almacenamiento y cámara, sírvela por HTTP local: desde esta carpeta ejecuta `python3 -m http.server 8000` y visita `http://localhost:8000`.
3. Entra en **Ajustes → Exportar todos los datos** periódicamente para mantener una copia de seguridad.

## Publicar en GitHub Pages
1. Crea un repositorio y sube `index.html`, `styles.css`, `app.js` y `README.md` a la raíz.
2. En el repositorio abre **Settings → Pages**.
3. Selecciona despliegue desde la rama principal y la carpeta raíz; guarda y espera a que GitHub publique el sitio.
4. Abre la URL publicada. Los datos se guardan en el navegador y origen donde se use la app; no se sincronizan entre dispositivos.

## Intercambio de archivos
- Las rutinas individuales usan `.gymlog`, un archivo JSON versionado que incluye las fotografías en formato de datos cuando existen.
- Las copias completas se exportan como JSON e incluyen rutinas, historial, preferencias y la sesión en curso. La importación permite añadir o reemplazar.

## Limitaciones de esta versión
- La persistencia es local al navegador y dispositivo. Borrar los datos del navegador puede eliminarlos.
- La fotografía utiliza el selector de archivos con sugerencia de cámara; el navegador decide si ofrece cámara directamente.
- La notificación sonora del temporizador depende de que el navegador permita iniciar audio.
- No hay sincronización en la nube ni funcionamiento sin conexión garantizado mediante caché de aplicación.
- Los archivos de rutina contienen JSON y datos de imagen incrustados; no se ejecuta código importado.

## Pruebas
- Comprobación sintáctica de `app.js` con `node --check`.
- Las rutinas iniciales, importación/exportación y almacenamiento se implementan en cliente. Se recomienda probar el flujo completo en los navegadores y móviles objetivo antes de usarlo como único registro.
