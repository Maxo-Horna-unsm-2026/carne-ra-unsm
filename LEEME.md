# Carné aumentado UNSM

Apunta la cámara del celular a la parte delantera del carné universitario y aparece, en 3D:

- Un marco dorado y una línea de escaneo sobre el carné.
- Una medalla 3D con el escudo de la UNSM que sale de la foto y gira.
- Una laptop 3D que se abre sobre el carné, con código en la pantalla.
- Un panel grueso con la facultad y la escuela profesional.
- 4 botones 3D (monedas) que se tocan para abrir: Intranet, Aula virtual, Biblioteca y Web UNSM.

El contenido usa un estabilizador: si mueves un poco el carné o la mano tiembla, el contenido se queda quieto. Si el carné se pierde un momento, el contenido espera casi 1 segundo antes de desaparecer.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La página (el código) |
| `targets.mind` | La "huella" del carné, para que la cámara lo reconozca |
| `escudo.png` | Escudo de la UNSM (pantalla de inicio) |
| `3d-*.jpg` y `3d-*.png` | Imágenes de los objetos 3D (medalla, laptop, panel, botones) |

## Publicar en GitHub Pages (10 minutos)

1. Entra a **github.com** e inicia sesión.
2. Arriba a la derecha toca **+** → **New repository**.
3. En *Repository name* escribe `carne-ra-unsm`. Deja marcado **Public**. Toca **Create repository**.
4. En la página que aparece, toca el enlace **uploading an existing file**.
5. Arrastra todos los archivos de la carpeta. Abajo toca **Commit changes**.
6. Ve a **Settings** (arriba) → **Pages** (menú de la izquierda).
7. En *Branch* elige **main** y la carpeta **/ (root)**. Toca **Save**.
8. Espera 1 o 2 minutos y recarga. Arriba aparecerá tu link:
   `https://TU-USUARIO.github.io/carne-ra-unsm/`

## Probar en el celular

1. Abre el link en **Chrome** (Android) o **Safari** (iPhone).
2. Toca **Comenzar** y luego **Permitir** cámara.
3. Apunta a la parte delantera del carné, a unos 20-30 cm.

Consejos:
- Usa buena luz y evita reflejos del plástico.
- Para probar sin carné, abre la foto del carné en la pantalla de la computadora y apunta el celular al monitor.
- Si cambias algún archivo en GitHub, espera 1 minuto y recarga la página en el celular.

## Cambios fáciles

- **Links de los logos:** en `index.html`, busca `data-url="..."` y cambia la dirección.
- **Estabilizador:** en `index.html`, busca `seguir-suave`. `zonaPos` y `zonaRot` son cuánto movimiento se ignora (más alto = más quieto); `rapidez` es qué tan rápido sigue al carné cuando sí se mueve.

## Problemas comunes

| Problema | Solución |
|---|---|
| No abre la cámara | El link debe empezar con `https://`. Revisa que el navegador tenga permiso de cámara. |
| No reconoce el carné | Más luz, menos reflejo, acércate o aléjate un poco. Usa el lado de adelante. |
| Pantalla en blanco | Revisa que todos los archivos estén subidos con esos nombres exactos (en minúsculas). |
