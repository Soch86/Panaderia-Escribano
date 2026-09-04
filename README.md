# Panadería Escribano – app de facturas (PWA)

Sin compilar nada. Sube esta carpeta a GitHub y publícala con GitHub Pages.

## Publicar (5 minutos)
1. En tu repositorio de GitHub, sube TODOS los archivos de esta carpeta (index.html, manifest.webmanifest, sw.js, icon-*.png).
   - Si los subes dentro de una subcarpeta (p. ej. /pwa), la dirección final llevará esa carpeta.
2. Settings → Pages → Source: "Deploy from a branch" → Branch: main, carpeta / (root o /docs según dónde los pusiste) → Save.
3. En 1-2 minutos tendrás la dirección: https://TU-USUARIO.github.io/TU-REPO/  (añade /pwa/ si la subiste ahí).

## Instalar en el móvil
- iPhone: abrir la dirección en Safari → Compartir → "Añadir a pantalla de inicio".
- Android: abrir en Chrome → menú ⋮ → "Instalar app" (o "Añadir a pantalla de inicio").

## Activar Google real (opcional)
1. console.cloud.google.com → nuevo proyecto → APIs y servicios → Habilitar "Google Drive API".
2. Credenciales → Crear credencial → ID de cliente OAuth → Aplicación web.
   - Orígenes autorizados de JavaScript: https://TU-USUARIO.github.io
3. Copia el Client ID y pégalo en index.html sustituyendo  window.__PWA__=true;  por  window.__PWA__=true;window.__GOOGLE_CLIENT_ID__='TU_CLIENT_ID';
   (o pásamelo y lo dejo puesto).

## Actualizar la app
Sustituye index.html por la nueva versión y sube el cambio. Los móviles la actualizan solas al abrirla.
