# Nido de Ideas

Sitio web del taller creativo **Nido de Ideas**: cerámica, ilustración y talleres presenciales.

## Sitio desplegado

El proyecto está publicado en GitHub Pages:

**https://pipodatabase.github.io/nido-de-ideas/**

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
└── images/
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
- SCSS (variables, mixins, nesting y partials) compilado a un único CSS
- Bootstrap 5.3.3 por CDN (navbar, carousel y acordeón)

Inicio, Proyectos y Servicios están adaptados a mobile y desktop. Sobre mí y Contacto mantienen contenido y estilos del resto del sitio.
