# GYM LOG

Aplicación web estática en español para crear rutinas, consultar ejercicios, registrar sesiones y exportar copias de seguridad. No requiere cuenta ni servidor propio.

## Archivos
- `index.html`: punto de entrada.
- `styles.css`: interfaz responsive.
- `app.js`: lógica de aplicación.
- `exercise-catalog.json`: catálogo inicial extraído de la especificación.
- `templates.json`: cuatro plantillas iniciales.

## Ejecutar localmente
Abre la carpeta con un servidor estático (recomendado, porque `fetch()` carga los JSON):
```bash
python3 -m http.server 8000
```
Después abre `http://localhost:8000`.

## Publicar en GitHub Pages
Sube todos los archivos de la carpeta a la raíz de la rama publicada (`main`, `/root`). La dirección habitual será `https://USUARIO.github.io/REPOSITORIO/`.

## Datos y privacidad
Los datos se guardan en IndexedDB y una copia auxiliar de compatibilidad en localStorage. No hay cuentas ni sincronización en la nube. Exporta copias desde Ajustes para mover datos entre dispositivos.

## Limitaciones conocidas de esta entrega
Es una base funcional de primera versión, no se afirma que haya superado las 50 pruebas completas de la especificación. El catálogo contiene los nombres y grupos/subgrupos extraídos del documento, pero aún no incluye fotografías precargadas ni descripciones/instrucciones detalladas para todos los ejercicios. El análisis de texto es local y basado en reglas, por lo que exige revisar los elementos pendientes de interpretar antes de guardar. Los gráficos son resúmenes sencillos, no un sistema estadístico avanzado.
