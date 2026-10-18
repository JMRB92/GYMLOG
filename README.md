# GYM LOG

Aplicación web estática en español para gestionar rutinas, consultar una biblioteca de ejercicios, registrar sesiones y exportar/importar datos. No necesita cuentas ni servicios externos. Los datos se almacenan localmente en IndexedDB del navegador.

## Archivos

Todos los archivos de la aplicación están en la raíz de esta carpeta: `index.html`, `styles.css`, `app.js`, `library.js` y `exercise-catalog.json`. El orden de scripts en `index.html` carga primero la biblioteca y después la aplicación.

## Publicar en GitHub Pages (sin compilar)

1. Descarga y descomprime el ZIP.
2. Abre el repositorio de GitHub y entra en **Code**.
3. Selecciona **Add file → Upload files**.
4. Arrastra los archivos de esta carpeta directamente a la raíz del repositorio (no arrastres la carpeta contenedora ni el ZIP).
5. Confirma los cambios con **Commit changes**.
6. Abre **Settings → Pages**.
7. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main` y carpeta `/(root)`. Pulsa **Save**.
8. Abre **Actions** y espera a que `pages build and deployment` termine en verde.
9. La URL habitual de un repositorio llamado `GYMLOG` en el usuario `JMRB92` es `https://jmrb92.github.io/GYMLOG/`.

Si anteriormente pulsaste **Unpublish site**, vuelve a Settings → Pages y guarda otra vez la configuración. No es necesario borrar el repositorio. Si la ejecución de Pages se cancela, abre el detalle de Actions para revisar el motivo; no vuelvas a subir los archivos repetidamente.

## Uso local

Para una prueba local fiable, abre un terminal en esta carpeta y ejecuta `python -m http.server 8000`; después visita `http://localhost:8000`.

## Privacidad y copias

- Los datos se guardan en el navegador y dispositivo donde se utiliza la aplicación. No hay sincronización automática entre dispositivos.
- Exporta periódicamente **Ajustes → Exportar todos los datos**.
- En **Historial** puedes descargar/compartir el historial y cargarlo más tarde.
- Las rutinas individuales se pueden exportar e importar mediante archivos `.gymlog`.
- Los archivos importados se leen como datos; no se ejecuta código que contengan.

## Alcance y pruebas

La aplicación incluye biblioteca de ejercicios, rutinas, registro de entrenamientos, historial, progreso básico y exportación/importación local. Se ha comprobado la sintaxis de JavaScript con `node --check`. Esta entrega no debe considerarse certificada para todos los 50 escenarios de la especificación: antes de depender de ella como único registro, prueba las operaciones principales en el móvil y navegador que vayas a utilizar. La conversión avanzada de rutinas desde texto, la PWA/offline completa y algunas reglas avanzadas de recuperación de sesiones pueden requerir desarrollo y pruebas adicionales.
