# Reloj Adaptable

App web instalable (PWA). Carga un fondo o una captura: el reloj elige el color y el contraste, y si la imagen trae hora y fecha, las reemplaza por la hora en vivo.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `reloj-adaptable`), público.
2. Sube **todo el contenido de esta carpeta** a la raíz del repositorio (`index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll` y la carpeta `icons/`).
3. En el repositorio entra a **Settings → Pages**. En *Build and deployment* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. Espera uno o dos minutos. La app queda en `https://TU-USUARIO.github.io/reloj-adaptable/`.

Con Git en la terminal:

```bash
git init -b main
git add .
git commit -m "Reloj Adaptable"
git remote add origin https://github.com/TU-USUARIO/reloj-adaptable.git
git push -u origin main
```

## Instalar en el celular

- **Android (Chrome):** abre la dirección, menú ⋮ → **Instalar app** (o *Añadir a pantalla de inicio*).
- **iPhone (Safari):** botón Compartir → **Añadir a pantalla de inicio**.

## Generar un APK (opcional)

Con la app ya publicada, entra a [pwabuilder.com](https://www.pwabuilder.com), pega la dirección y elige **Android** para descargar el paquete.

## Notas

- La lectura automática de la hora y la fecha en capturas necesita internet la primera vez (descarga el lector de texto). Si falla, usa *Marcar hora a mano* y *Marcar fecha a mano*.
- Las imágenes se procesan en el dispositivo y no se envían a ningún servidor.
- Para publicar un cambio, edita `index.html` y cambia el número de `CACHE` en `sw.js`.

Dirección de la app: https://reneyacoinfa11-lab.github.io/reloj-adaptable/
