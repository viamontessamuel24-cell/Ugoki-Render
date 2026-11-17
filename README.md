# Ugoki

App Android (Kotlin + Jetpack Compose) que convierte animaciones HTML/CSS/JS en MP4 2K.

## Compilar en GitHub
1. Sube todo este proyecto a un repositorio (incluida la carpeta `.github/workflows/build.yml`).
2. Pestaña **Actions** → workflow **Build APK** (corre solo con cada push).
3. Al terminar, descarga el artefacto **Ugoki-debug-apk** e instala el APK.

## Notas para tus HTML
- Un solo archivo .html (CSS y JS dentro). Librerías por CDN https (GSAP, etc.) funcionan con internet.
- Override opcional en `<head>`:
  - `<meta name="ugoki-format" content="9:16">` (o `16:9`)
  - `<meta name="ugoki-duration" content="8">` (segundos)
- Salida: Películas/Ugoki (2K 60 FPS si el chip lo soporta; si no, baja a 2K30 → 1080p60 → 1080p30).
