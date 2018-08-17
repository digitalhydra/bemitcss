# NPM script build process

Procesador de maquetacion en sass con auto refresh en broserify
y proceso de construcion para produccion

### Instalacion

```
npm install
```
Para instalar dependencias
```
npm run dev
```
para correr en navegador

```
npm run build
```
para para construir version minificada de estilos `dist/css/main.min.css`

```
npm run styleguide
```
para para generar el styleguide es necesario generar primero el `build`

####Estructura del styleguide

- /settings: Global variables, site-wide settings, config switches, etc.
- /tools: Site-wide mixins and functions.
- /generic: Low-specificity, far-reaching rulesets (e.g. resets).
- /elements: Unclassed HTML elements (e.g. a {}, blockquote {}, address {}).
- /objects: Objects, abstractions, and design patterns (e.g. .o-layout {}).
- /components: Discrete, complete chunks of UI (e.g. .c-carousel {}). This is the one layer that inuitcss doesn’t provide code for, as this is completely your terrain.
- /utilities: High-specificity, very explicit selectors. Overrides and helper classes (e.g. .u-hidden {}).
- /views (optional): se crearan los estilos especificos para cada pantalla. (e.g. .v-listado-proyectos)