# Carné aumentado UNSM

Apunta la cámara del celular a la parte delantera del carné universitario y aparecen, en realidad aumentada:

- Un marco dorado y una línea de escaneo sobre el carné.
- El escudo, que sale de la zona de la foto y se balancea.
- Un panel con la facultad y la escuela profesional.
- 4 botones: Intranet, Aula virtual, Biblioteca y Web UNSM.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La página (el código) |
| `targets.mind` | La "huella" del carné, para que la cámara lo reconozca |
| `escudo.png` | El escudo que aparece en RA (provisional) |
| `panel-facultad.png` | El panel de la facultad |

## Publicar en GitHub Pages (10 minutos)

1. Entra a **github.com** e inicia sesión.
2. Arriba a la derecha toca **+** → **New repository**.
3. En *Repository name* escribe `carne-ra-unsm`. Deja marcado **Public**. Toca **Create repository**.
4. En la página que aparece, toca el enlace **uploading an existing file**.
5. Arrastra los 4 archivos (`index.html`, `targets.mind`, `escudo.png`, `panel-facultad.png`). Abajo toca **Commit changes**.
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

- **Escudo oficial:** reemplaza `escudo.png` por el escudo real de la UNSM (PNG con fondo transparente, más alto que ancho) con **el mismo nombre**.
- **Links de los botones:** en `index.html`, busca `<div id="accesos">` y cambia las direcciones `href="..."`.
- **Si el contenido tiembla:** en `index.html`, en `filterBeta: 0.001`, prueba con `0.0001`.

## Problemas comunes

| Problema | Solución |
|---|---|
| No abre la cámara | El link debe empezar con `https://`. Revisa que el navegador tenga permiso de cámara. |
| No reconoce el carné | Más luz, menos reflejo, acércate o aléjate un poco. Usa el lado de adelante. |
| Pantalla en blanco | Revisa que los 4 archivos estén subidos con esos nombres exactos (en minúsculas). |
