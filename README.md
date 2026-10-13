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
│   ├── colores.scss
│   ├── general.scss
│   ├── header.scss
│   ├── botones.scss
│   ├── contenido.scss
│   ├── footer.scss
│   └── estilos.scss
├── css/
│   └── estilos.css
└── README.md
```

## Tecnologías utilizadas

- HTML5
- CSS3
- Sass (SCSS)
- Visual Studio Code

## Páginas web

- **Inicio (`index.html`):** presentación del portfolio y proyectos destacados.
- **Sobre mí (`sobre.html`):** información personal y habilidades.
- **Contacto (`contacto.html`):** formulario de contacto.

## Compilación de Sass

Para generar el archivo CSS a partir del SCSS, utilizo el siguiente comando:

```bash
sass --watch scss/estilos.scss:css/estilos.css
```

El archivo `estilos.css` será compartido por las tres páginas HTML.

## Validación

Se comprobará que el CSS generado no contenga errores mediante este validador oficial:

https://jigsaw.w3.org/css-validator/

## Autor

 Pepe Gil Cué - Estudiante del ciclo formativo de Desarrollo de Aplicaciones Web (DAW).

## Módulo

Diseño de Interfaces Web (DIW) — UD2: Uso de Estilos.
