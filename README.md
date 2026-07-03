# Café Grulla ☕

App web para gestionar las ventas de café de especialidad: clientes, catálogo de cafés, pedidos (con varios cafés por venta), estado de entrega y de pago, y un resumen de pendientes. Los datos se guardan localmente en el dispositivo.

Es una **PWA**: se puede instalar en el teléfono como una app (con ícono y pantalla de entrada) y funciona sin conexión.

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub y subí **todos** estos archivos, respetando la estructura:

   ```
   index.html
   support.js
   manifest.webmanifest
   sw.js
   .nojekyll
   icons/
     logo.png
     icon-192.png
     icon-512.png
     icon-maskable-512.png
     apple-touch-icon.png
   ```

2. En el repo: **Settings → Pages**.
3. En *Build and deployment → Source* elegí **Deploy from a branch**.
4. Branch: **main** (o `master`), carpeta **/ (root)**. Guardá.
5. Esperá ~1 minuto. GitHub te dará una URL tipo:
   `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`

## Instalar en el teléfono

1. Abrí esa URL en **Chrome (Android)** o **Safari (iPhone)**.
2. **Android:** menú ⋮ → *Instalar app* / *Agregar a pantalla de inicio*.
3. **iPhone:** botón *Compartir* → *Agregar a inicio*.
4. Va a aparecer con el ícono de la grulla y su pantalla de entrada al abrir.

> Nota: la instalación como app y el funcionamiento sin conexión requieren HTTPS, que GitHub Pages ya provee. Abrir el `index.html` directo desde el disco funciona, pero sin instalación ni offline.

## Guardado de datos

Clientes, cafés y ventas se guardan en el navegador del dispositivo (localStorage). No se sincronizan entre teléfonos.
