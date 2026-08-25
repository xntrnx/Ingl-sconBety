# Test de ubicación de inglés — sitio estático

Dos páginas planas, sin backend:
- `index.html` — el test de nivel (9 preguntas → resultado → canales de venta)
- `profesora.html` — portafolio de la Mtra. Beatriz Mendoza

## Antes de subir

Reemplaza los marcadores de posición:
- En `index.html`: los links de WhatsApp (`52XXXXXXXXXX`), Instagram (`TU_USUARIO`) y correo.
- En `profesora.html`: los textos en cursiva entre corchetes (trayectoria, cita, cursos) y el número de WhatsApp.

## Subir a GitHub (primera vez)

1. Instala Git si no lo tienes: https://git-scm.com
2. Crea una cuenta en https://github.com si no tienes.
3. Crea un repositorio nuevo en GitHub (botón "New repository"). Ponle un nombre, por ejemplo `test-de-nivel`. No marques "Add a README" (ya tienes uno).
4. En tu terminal, dentro de esta carpeta:
   ```
   git init
   git add .
   git commit -m "Sitio del test de nivel"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/test-de-nivel.git
   git push -u origin main
   ```
   (Reemplaza `TU_USUARIO` y el nombre del repo por los tuyos — GitHub te los muestra en la página del repo recién creado, en el botón "Code".)

## Publicarlo con GitHub Pages (gratis)

1. En GitHub, entra a tu repo → pestaña **Settings** → sección **Pages** (menú de la izquierda).
2. En "Build and deployment" → "Source", elige **Deploy from a branch**.
3. En "Branch", selecciona `main` y la carpeta `/ (root)`. Guarda.
4. Espera 1–2 minutos. GitHub te da una URL tipo:
   ```
   https://TU_USUARIO.github.io/test-de-nivel/
   ```
   Ahí vive `index.html` (el test), y `https://TU_USUARIO.github.io/test-de-nivel/profesora.html` es el portafolio — el link entre ambas páginas ya funciona porque están en la misma carpeta.

## Cuando hagas cambios después

Cada vez que edites algo localmente:
```
git add .
git commit -m "Descripción del cambio"
git push
```
GitHub Pages se actualiza solo, unos minutos después de cada push.
