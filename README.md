# Consultas de Odontopediatría · Juego 2D sobre caries

Este juego educativo se abre en el navegador y no necesita instalación. Tiene tres casos ficticios: Valentina (3 años), Mateo (7) y Camila (14). En cada caso el estudiante recorre una clínica 2D y toma 5 decisiones con 10 fichas de tiempo clínico. Cada decisión muestra su consecuencia. Al final escribe una justificación y ve su progreso en «Mi avance».

Incluye narración bilingüe (ElevenLabs y voz neuronal), alto contraste, tamaño de texto ajustable y juego completo con teclado. Guía 25 · Vibe Coding CEDIA 2026.

## Archivos

| Archivo | Para qué |
|---|---|
| `index.html` | El juego completo. El audio va incrustado, así que es un solo archivo de unos 8 MB. |
| `.nojekyll` | Hace que GitHub Pages publique los archivos tal cual. |
| `reglas.md` | La especificación: tarjetas, costos, puntos, consecuencias y versión. |
| `partidas_referencia.csv` | Tres estrategias por caso, calculadas a mano, para verificar el juego. |
| `Code.gs` | Receptor para la hoja de Google, con las pestañas Resultados, Acumulado y Avance. |
| `INSTRUCCIONES_hoja_google.md` | Cómo conectar la hoja de Google (10 minutos). |
| `guion_narracion.md`, `guion_microrecurso.md` | Guiones bilingües de la narración. |
| `PLAN.md` | Plan de construcción y pruebas de aceptación (guía 25). |

## Publicar en GitHub Pages (desde el navegador, sin instalar nada)

1. Entre a https://github.com con su cuenta y pulse **New repository**. Nombre sugerido: `juego-caries`. Elija **Public**, porque GitHub Pages gratuito requiere repositorio público, y pulse **Create repository**.
2. En la página del repositorio vacío pulse **uploading an existing file**. Arrastre **todos** los archivos de esta carpeta, incluido `.nojekyll`. Si el explorador oculta ese archivo, puede omitirlo. Pulse **Commit changes**.
3. Vaya a **Settings › Pages**. En *Build and deployment* elija **Deploy from a branch**, rama **main**, carpeta **/ (root)**, y pulse **Save**.
4. Espere 1 o 2 minutos y recargue la página. Arriba aparece el enlace `https://<su-usuario>.github.io/juego-caries/`. Ese es el enlace que comparte con los estudiantes, o que pega en Moodle o Canvas como recurso URL.

Para actualizar el juego, suba de nuevo `index.html` con **Add file › Upload files**. El enlace no cambia.

## Conectar la hoja de Google

Siga `INSTRUCCIONES_hoja_google.md`. Al final pegue la URL `/exec` en la línea `const URL_HOJA_GOOGLE = "";` de `index.html` y vuelva a subir el archivo.

## Privacidad

- El juego no pide nombres ni cédula, solo un código anónimo, por ejemplo `P-014`.
- El avance del estudiante se guarda en su propio navegador.
- A la hoja del docente llega solamente lo que el estudiante calcula después de aceptar el consentimiento.

Los casos son ficticios. Los puntos son reglas educativas, no predicciones clínicas.
