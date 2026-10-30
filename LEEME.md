# Chatbot & Marca · Cómo publicarlo en GitHub Pages

Un solo repositorio, una sola publicación y un enlace distinto para cada misión.

## Qué hay en esta carpeta

- `mision-1.html` a `mision-8.html`: una página por misión. Cada una tiene su propio enlace.
- `ds/`, `assets/`, `support.js`, `image-slot.js`: estilos, fuentes, imágenes y funcionamiento que comparten las 8 misiones. No los borres ni los renombres.
- `.nojekyll`: archivo oculto y vacío, necesario para que GitHub publique la carpeta `ds`. No lo borres.

Subes **una sola carpeta** y obtienes **8 enlaces**, uno por misión.

## Paso a paso

### 1. Crea el repositorio (una sola vez)
1. Entra a github.com con la cuenta de CTC.
2. Arriba a la derecha toca **+ › New repository**.
3. En **Repository name** escribe un nombre corto y sin espacios, por ejemplo `chatbot-y-marca`.
4. Marca **Public**. GitHub Pages gratis solo publica repositorios públicos.
5. Toca **Create repository**.

### 2. Sube los archivos
1. En el repositorio nuevo, toca **uploading an existing file**, o **Add file › Upload files**.
2. Abre la carpeta `publicar` en tu computadora, selecciona **todo su contenido** (no la carpeta en sí) y arrástralo a la ventana de GitHub.
   - En Mac, presiona `Cmd + Shift + .` para ver y arrastrar también `.nojekyll`.
   - En Windows, activa Vista › Elementos ocultos.
   - Si GitHub no toma `.nojekyll`, créalo ahí mismo: **Add file › Create new file**, ponle el nombre `.nojekyll` y guárdalo vacío.
3. Revisa que arriba se vean las carpetas `ds` y `assets` y los archivos `mision-1.html` … `mision-8.html`.
4. Abajo toca **Commit changes**.

### 3. Publica con GitHub Pages
1. En el repositorio toca **Settings › Pages** (en el menú de la izquierda).
2. En **Source** elige **Deploy from a branch**.
3. En **Branch** elige `main` y la carpeta `/ (root)`. Toca **Save**.
4. Espera 1 o 2 minutos y recarga la página. Arriba aparecerá: *Your site is live at…*

### 4. Tus enlaces
La dirección base de tu sitio es `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`. A esa dirección le agregas el nombre de cada misión. Por ejemplo, si tu usuario es `ctc-usuario` y el repositorio `chatbot-y-marca`:

| Página | Enlace |
|---|---|
| Misión 1 | https://ctc-usuario.github.io/chatbot-y-marca/mision-1.html |
| Misión 2 | https://ctc-usuario.github.io/chatbot-y-marca/mision-2.html |
| Misión 3 | https://ctc-usuario.github.io/chatbot-y-marca/mision-3.html |
| Misión 4 | https://ctc-usuario.github.io/chatbot-y-marca/mision-4.html |
| Misión 5 | https://ctc-usuario.github.io/chatbot-y-marca/mision-5.html |
| Misión 6 | https://ctc-usuario.github.io/chatbot-y-marca/mision-6.html |
| Misión 7 | https://ctc-usuario.github.io/chatbot-y-marca/mision-7.html |
| Misión 8 | https://ctc-usuario.github.io/chatbot-y-marca/mision-8.html |

Cambia `ctc-usuario` y `chatbot-y-marca` por los tuyos. La dirección base sola (sin `mision-X.html`) mostrará un error 404, y es normal: no hay portada.

### 5. Ponlo en Moodle / Campus CTC
- **Como enlace:** en cada sesión, agrega un recurso **URL** con el enlace de esa misión y elige que se abra en una ventana nueva.
- **Incrustado:** en una página o etiqueta, usa el editor HTML y pega:
  `<iframe src="ENLACE-DE-LA-MISION" width="100%" height="800" style="border:0" allowfullscreen></iframe>`
  Si la pantalla completa o el botón de copiar no funcionan dentro del iframe, usa la opción de enlace.

## Cómo actualizar una misión después
1. Entra al repositorio y abre, por ejemplo, `mision-3.html`.
2. Toca **Add file › Upload files**, arrastra la versión nueva con **el mismo nombre** y toca **Commit changes**.
3. En 1 o 2 minutos el enlace muestra la versión nueva. El enlace no cambia.
4. Para cambiar una imagen, sube la nueva a `assets/img/` con el mismo nombre.

## Si algo no se ve bien
- **Página en blanco o sin estilos:** falta `.nojekyll`, o la carpeta `ds` no se subió completa.
- **Error 404:** revisa que el nombre del archivo sea exactamente `mision-1.html` (en minúsculas y sin espacios), y espera 2 minutos después de cada cambio.
- **Imágenes rotas:** revisa que exista `assets/img/` con todas las imágenes.
