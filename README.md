# Proyecto Refactorizado

## Descripción

Actividad práctica del módulo de Diseño de Interfaces Web (DIW) cuyo objetivo es refactorizar una página web personal tipo portfolio, separando el contenido HTML de los estilos CSS mediante Sass (SCSS).

## Objetivos

- Eliminar los estilos en línea y los bloques de estilos internos.
- Utilizar HTML semántico.
- Centralizar los estilos en una única hoja CSS externa.
- Organizar los estilos mediante archivos parciales SCSS.
- Mantener un diseño coherente en las tres páginas.
- Crear un formulario de contacto.
- Validar el CSS generado.

## Estructura del proyecto

```text
proyecto-refactorizado/
├── index.html
├── sobre.html
├── contacto.html
├── scss/
│   ├── _colores.scss
│   ├── _general.scss
│   ├── _header.scss
│   ├── _botones.scss
│   ├── _contenido.scss
│   ├── _footer.scss
│   └── estilos.scss
├── css/
│   └── estilos.css
└── README.md
```

`estilos.scss` importa todos los parciales con `@import`. Los parciales llevan guion bajo para que Sass no genere un CSS por cada uno.

## Tecnologías utilizadas

- HTML5
- CSS3
- Sass (SCSS)
- Visual Studio Code

## Páginas web

- **Inicio (`index.html`):** presentación del portfolio y proyectos destacados.
- **Sobre mí (`sobre.html`):** información personal y habilidades.
- **Contacto (`contacto.html`):** formulario de contacto.

## Cómo ver el proyecto

Abrir `index.html` en el navegador (o usar la extensión Live Server de VS Code).

## Compilación de Sass

Instalar Sass (una sola vez):

```bash
npm install -g sass
```

Compilar una vez:

```bash
sass scss/estilos.scss css/estilos.css
```

O compilar automáticamente al guardar:

```bash
sass --watch scss/estilos.scss:css/estilos.css
```

El archivo `estilos.css` es compartido por las tres páginas HTML.

## Validación

El CSS generado se comprueba con el validador oficial del W3C:

https://jigsaw.w3.org/css-validator/

## Autor

Pepe Gil Cué - Estudiante del ciclo formativo de Desarrollo de Aplicaciones Web (2ªDAW).

## Módulo

Diseño de Interfaces Web (DIW) — UD2: Uso de Estilos.
