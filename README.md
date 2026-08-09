# Veritas Academy — Plataforma Escolar

Sitio estático de 5 páginas, listo para publicarse en GitHub Pages.

## Estructura

```
index.html          → Panel administrativo (página de inicio)
escaner.html         → Escáner de acceso (voz + idioma + modo offline)
registro.html        → Registro de alumno (foto/QR + idioma + modo offline)
configuracion.html   → Configuración de la escuela (logo, datos institucionales)
encuestas.html       → Portal de encuestas para padres
assets/logo.png      → Logo institucional
assets/photo-placeholder.svg → Ícono usado antes de subir una foto de alumno
README.md            → Este archivo
```

Todas las páginas están enlazadas entre sí con navegación real (barra superior,
menú lateral en escritorio y barra inferior en móvil).

## Publicar en GitHub Pages

1. En tu repositorio de GitHub, sube **todo el contenido de esta carpeta**
   directamente en la raíz del repositorio (no dentro de una subcarpeta),
   respetando que `index.html` quede en la raíz junto con la carpeta `assets/`.

   Con git desde tu computadora:
   ```bash
   cd carpeta-donde-descomprimiste-el-sitio
   git init
   git add .
   git commit -m "Publicar plataforma Veritas Academy"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/TU-REPOSITORIO.git
   git push -u origin main
   ```
   (Si el repositorio ya existía con otros archivos, usa `git add .` y
   `git commit` normalmente sobre lo que ya tengas clonado.)

2. En GitHub, entra a tu repositorio → **Settings** → **Pages**.

3. En "Build and deployment" → "Source", selecciona **Deploy from a branch**.

4. En "Branch", selecciona **main** y la carpeta **/ (root)** → **Save**.

5. Espera 1-2 minutos. GitHub te dará una URL parecida a:
   `https://TU-USUARIO.github.io/TU-REPOSITORIO/`

   Esa URL abrirá directamente `index.html` (el panel administrativo).

## Notas importantes

- El sitio funciona sin backend: el registro de alumnos y el escáner guardan
  los datos en el propio dispositivo (localStorage), pensado para escuelas
  sin conexión estable a internet. Esos datos **no se sincronizan solos entre
  dispositivos** — quedan guardados en el navegador donde se capturaron.
- El logo se puede reemplazar desde `configuracion.html`: al subir uno nuevo,
  se guarda en el navegador y se aplica automáticamente en el resto de las
  páginas (mismo dispositivo/navegador).
- Como es un sitio estático, cualquier imagen nueva que subas desde el
  navegador (logo, fotos de alumnos) vive únicamente en ese navegador —
  no se sube sola a GitHub. Si quieres una imagen fija disponible para todos
  (por ejemplo, el logo definitivo), lo más simple es reemplazar el archivo
  `assets/logo.png` en el repositorio y volver a publicar.
