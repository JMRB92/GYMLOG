# GYM LOG

Aplicación web para crear y editar rutinas de gimnasio, registrar entrenamientos y consultar el historial. Está construida con HTML, CSS y JavaScript sin dependencias externas ni servidor: puedes ejecutarla localmente o publicarla gratis con **GitHub Pages**.

## Probar la aplicación

1. Descarga este repositorio o abre `index.html` en un navegador moderno.
2. Crea o selecciona una rutina y registra una sesión.
3. Los datos se guardan en el almacenamiento local (`localStorage`) de ese navegador y dispositivo.

> **Importante:** los datos no se sincronizan entre dispositivos ni se guardan en GitHub. Exporta copias de seguridad desde la aplicación antes de borrar los datos del navegador o cambiar de dispositivo. No uses el modo privado si necesitas conservar los datos.

## Publicarla en GitHub Pages

### Opción A: subir los archivos desde la web de GitHub

1. Entra en [GitHub](https://github.com/) e inicia sesión.
2. Pulsa **New repository**.
3. Pon como nombre `gym-log` (o el que prefieras). Puedes marcarlo como **Public** y crear el repositorio. No necesitas añadir README, licencia ni `.gitignore` desde GitHub porque ya están incluidos aquí.
4. En el repositorio, pulsa **Add file → Upload files**.
5. Sube **el contenido** de esta carpeta: `index.html`, `README.md`, `LICENSE`, `CHANGELOG.md`, `CONTRIBUTING.md`, `SECURITY.md`, `.nojekyll`, `favicon.svg`, `manifest.webmanifest`, `robots.txt`, `.gitignore` y la carpeta `.github` con su flujo de trabajo.
6. Pulsa **Commit changes**.
7. Abre **Settings → Pages**. En **Build and deployment**, selecciona **GitHub Actions** si no se ha seleccionado automáticamente.
8. Abre la pestaña **Actions** y espera a que termine correctamente el flujo **Deploy GYM LOG to GitHub Pages**.
9. La dirección será `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/`. Si el repositorio se llama `gym-log`, por ejemplo, la ruta termina en `/gym-log/`.

### Opción B: con Git en el ordenador

Descarga y descomprime el ZIP, abre una terminal dentro de la carpeta y ejecuta:

```bash
git init
git add .
git commit -m "Publica GYM LOG"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/NOMBRE-DEL-REPOSITORIO.git
git push -u origin main
```

Sustituye `TU-USUARIO` y `NOMBRE-DEL-REPOSITORIO` por los valores reales. Si el repositorio ya tiene commits o archivos, revisa su estado antes de ejecutar estos comandos para no sobrescribir trabajo.

## Qué incluye

- Cuatro rutinas de ejemplo editables.
- Registro de series, repeticiones y peso.
- Recuperación de valores de una sesión anterior compatible.
- Guardado automático local y reanudación de sesiones interrumpidas.
- Temporizador de descanso con ajustes.
- Biblioteca de ejercicios, búsqueda y ejercicios personalizados.
- Edición de rutinas, días y ejercicios.
- Importación de rutinas desde texto con vista previa.
- Historial y estadísticas básicas.
- Exportación e importación de copias de seguridad.
- Flujo de GitHub Actions para publicar en GitHub Pages.

## Privacidad y límites actuales

- La aplicación no necesita cuenta, backend ni conexión a una API externa.
- Los registros se guardan en el almacenamiento local del navegador. Borrar los datos del sitio puede eliminarlos.
- No existe sincronización en la nube, inicio de sesión, base de datos remota ni recuperación de datos perdidos.
- Esta versión no implementa una PWA completa ni garantiza funcionamiento instalable/offline mediante service worker.
- El flujo de publicación no sustituye las pruebas manuales en distintos navegadores y móviles.

## Estructura

```text
GYM_LOG_GitHub/
├── .github/workflows/deploy-pages.yml
├── .gitignore
├── .nojekyll
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── SECURITY.md
├── favicon.svg
├── index.html
├── manifest.webmanifest
└── robots.txt
```

## Licencia

Distribuido bajo la licencia MIT. Consulta `LICENSE`.
