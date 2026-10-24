# Nido de Ideas

Sitio web del taller creativo **Nido de Ideas**: cerámica, ilustración y talleres presenciales.

## Sitio desplegado

El proyecto está publicado en Vercel:

**https://tarea-self-one.vercel.app**

## Repositorio

**https://github.com/PipoDataBase/nido-de-ideas**

## Páginas

- [Inicio](index.html)
- [Sobre mí](pages/sobre-mi.html)
- [Proyectos](pages/proyectos.html)
- [Servicios](pages/servicios.html)
- [Contacto](pages/contacto.html)

## Estructura

```
nido-de-ideas/
├── index.html
├── pages/
│   ├── sobre-mi.html
│   ├── proyectos.html
│   ├── servicios.html
│   └── contacto.html
├── scss/
│   ├── main.scss
│   ├── utilities/
│   │   ├── _variables.scss
│   │   └── _mixins.scss
│   ├── base/
│   │   ├── _tipografia.scss
│   │   └── _base.scss
│   ├── layout/
│   │   ├── _header.scss
│   │   ├── _footer.scss
│   │   └── _nav.scss
│   └── components/
│       ├── _buttons.scss
│       ├── _cards.scss
│       ├── _sections.scss
│       ├── _grids.scss
│       ├── _forms.scss
│       ├── _gallery.scss
│       └── _accordion.scss
├── styles/
│   └── styles.css
└── assets/
```

`styles/styles.css` no se edita a mano: es la compilación de `scss/main.scss`. Los cinco HTML siguen enlazando esa hoja y el CDN de Bootstrap.

## Compilar los estilos

Hace falta Node.js. Desde la raíz del proyecto:

```bash
npm install
npm run build
```

Para recompilar solo mientras se editan los partials: `npm run watch`.

## Tecnologías

- HTML5 semántico
- SCSS compilado a un único CSS: variables, nesting, mixins con parámetros, `@extend` y operadores
- Animación nativa con `@keyframes` en el logotipo y `transition` en los controles
- AOS por CDN para la entrada de secciones, tarjetas y figuras
- Bootstrap 5.3.3 por CDN (navbar, carousel y acordeón)

Las cinco páginas están pensadas mobile-first y se reacomodan en tablet (`768px`) y escritorio (`1024px`).
