# Silas Vance — Análisis táctico de Lexington Sporting Club

Portafolio bilingüe (ES/EN) de análisis táctico de **Lexington Sporting Club** (USL Championship), publicado con GitHub Pages.
Autor: Alejandro Mena · Redes: [Instagram](https://www.instagram.com/silasperformancelsc) · [TikTok](https://www.tiktok.com/@silasperformancelsc)

## Estructura

```
index.html                  Portada del portafolio (enlaza todas las páginas)
images/                     Imágenes del sitio (foto de perfil)
analisis/
├── pre/                    Pre-partido  → AAAA-MM-DD-rival.html
├── post/                   Post-partido → AAAA-MM-DD-rival.html
├── jugadores/              Player Focus → apellido.html
├── equipo/                 Análisis de equipo / patrones
├── video-pending.html      Página de "video en producción" (se usa en los botones de video)
└── *.html                  Redirecciones de URLs antiguas (no editar; ver abajo)
```

## Cómo agregar una página nueva

1. Nombra el archivo según la carpeta:
   - Pre-partido: `analisis/pre/2026-10-17-rival.html`
   - Post-partido: `analisis/post/2026-10-17-rival.html`
   - Jugador: `analisis/jugadores/apellido.html`
   - Equipo: `analisis/equipo/tema.html`
2. Dentro de la página, los enlaces de vuelta al portafolio van con dos niveles: `../../index.html#pre-match` (o `#post-match`, `#individual`, `#team-tactics`).
   La página de video pendiente es `../video-pending.html`.
3. Cada página lleva un **id raíz único** que agrupa todo su CSS, para evitar colisiones.
4. Agrega la tarjeta en `index.html` dentro de la sección correspondiente (y en *Track record* si es pre-partido).
5. Reemplaza `PEGAR_ENLACE_VIDEO`, `PEGAR_ENLACE_INSTAGRAM` y `PEGAR_ENLACE_TIKTOK` cuando el video esté publicado.

## Redirecciones

Los archivos sueltos en `analisis/` (por ejemplo `pre-fctulsa.html` o `post-elpaso.html`) son las URLs de antes de la reorganización.
Cada uno redirige automáticamente a su nueva ubicación y conserva `?lang=` y `#ancla`, para que los links ya compartidos en redes sigan funcionando.
No pongas contenido nuevo ahí.

## Sistema de diseño

Verde `#3DDC5A` (acento / victorias) · Negro `#111111` (derrotas / alerta) · Hueso `#F5F1E9` (texto) · Fondo `#0B0F0C` · Panel `#131A14`
Fuentes: Oswald (títulos), Inter (cuerpo), IBM Plex Mono (etiquetas).
