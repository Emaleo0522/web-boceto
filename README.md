# Stanley Argentina — Landing Page

Landing page premium para tienda de termos, mates y accesorios Stanley. Diseñada como template de e-commerce de producto único, con animaciones GSAP, mosaico de videos y diseño totalmente responsive.

## Demo

[web-boceto.vercel.app](https://web-boceto.vercel.app)

## Características

- **Hero animado** — Mosaico de videos de productos en columnas verticales + animación de texto con GSAP (word reveal con blur y rotación 3D)
- **Catálogo con tabs** — Secciones Termos / Mates / Bombillas con cards y hover overlay
- **Galería expandible** — Efecto flex-expand al hacer hover sobre cada ítem
- **Testimonios** — Cards con blockquote, avatar circular y rating de estrellas
- **About con stats** — Contadores animados al entrar al viewport (IntersectionObserver)
- **Feature cards** — Cards con shimmer hover y badges emergentes
- **FAQ accordion** — Preguntas frecuentes con toggle CSS
- **Header fijo** — Con glassmorphism (backdrop-filter) y scroll behavior
- **100% Responsive** — Mobile, tablet y desktop

## Stack

- HTML5 + CSS3 vanilla (sin frameworks)
- GSAP 3.12 para animaciones
- Font Awesome 4.5 para íconos
- Un solo archivo `index.html` (zero build step)
- Deploy: Vercel (drop estático)

## Estructura

```
web-boceto/
├── index.html              # App completa (HTML + CSS + JS inline)
├── pareja-abrazandose-...  # Imagen hero
├── 813b07134956809...png   # Imagen de marca (fondo About, opacity 4%)
├── 13459051_720_1280_30fps.mp4
├── 14217640-hd_720_1280_60fps.mp4
├── 19314935-hd_720_1280_30fps.mp4
└── 6912128-hd_720_1280_25fps.mp4
```

## Uso como template

Las variables de marca están centralizadas en `:root`:

```css
:root {
  --stanley-green: #2d5b3f;
  --stanley-light-green: #4a7c5c;
  --stanley-yellow: #ffd700;
  /* ... */
}
```

Para adaptarlo a otra marca: cambiar los colores en `:root`, reemplazar los videos/imágenes y actualizar los textos del HTML.

## Pendiente / TODOs

- [ ] Hamburger menu para mobile (nav oculto en pantallas < 768px)
- [ ] Imágenes de productos reales (actualmente usa placeholders con gradientes)
- [ ] Galería con imágenes reales de productos
- [ ] Optimizar videos (WebM + lazy loading)
- [ ] Agregar SEO meta tags (OG, Twitter cards)
