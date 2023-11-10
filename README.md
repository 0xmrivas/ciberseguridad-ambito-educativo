# Documentación uniforme

## Diapositivas

En la carpeta [slides](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/main/slides) hay dos presentaciones de diapositivas de ejemplo, [example.html](https://crispy-carnival-8f8f6875.pages.github.io/slides/example.html) y [slides1.html](https://crispy-carnival-8f8f6875.pages.github.io/slides/slides1.html). Ambas están escritas usando RevealJS, configuradas para construir el contenido en base a un archivo Markdown. En concreto, [example.html](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/slides/example.html) renderiza el contenido de [example.md](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/slides/example.md) y [slides1.html](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/slides/slides1.html) renderiza el contenido de [slides1.md](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/slides/slides1.md). Puedes copiar cualquiera de los dos HTML para crear nuevas presentaciones de diapositivas. Solamente tienes que abrirlo y modificar el archivo .md del que quieres que coja la información.

Cada vez que se realiza una modificación en la carpeta slides, se ejecuta una Github Action ([slides-to-pdf](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/.github/workflows/slides-to-pdf.yml)) que genera las presentaciones en archivo PDF dentro de la rama [exports](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/exports). Puedes modificar el Github Action para ejecutarlo de forma manual cuando quieras o para que solo genere el PDF de ciertas presentaciones concretas.

Si está activo [Github Pages](https://github.com/IES-Rafael-Alberti/uniform-documentation/settings/pages) en el repositorio, podrás acceder a la presentación de diapositivas simplemente escribiendo: [URL_GITHUB_PAGES_REPOSITORIO]/slides/[NOMBRE_PRESENTACION].html.

Por ejemplo:

- https://crispy-carnival-8f8f6875.pages.github.io/slides/example.html ➝ Echa un vistazo para ver ejemplos de lo que puede hacerse con RevealJS y un archivo Markdown
- https://crispy-carnival-8f8f6875.pages.github.io/slides/slides1.html

## Documentos (descripciones de proyectos, apuntes...)

En la carpeta [docs](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/main/docs) hay dos documentos de ejemplo, [proyecto1.md](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/docs/proyecto1.md)) y [proyecto2.md](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/docs/proyecto2.md). Ambos son archivos escritos en Markdown. Puedes crear todos los archivos .md que quieras en esta carpeta para añadir nuevas descripciones o apuntes.

Cada vez que se realiza una modificación en la carpeta docs, se ejecutan dos Github Actions, [docs-to-html](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/.github/workflows/docs-to-html.yml) y [docs-to-pdf](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/.github/workflows/docs-to-pdf.yml). El primero genera un archivo .html de los documentos .md enlazando una hoja de estilos CSS, dentro de la misma carpeta docs. El segundo genera los archivos PDF de los documentos .md usando la misma hoja de estilos dentro de la rama [exports](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/exports).

Si está activo [Github Pages](https://github.com/IES-Rafael-Alberti/uniform-documentation/settings/pages) en el repositorio, podrás acceder a la versión HTML de los documentos simplemente escribiendo: [URL_GITHUB_PAGES_REPOSITORIO]/docs/[NOMBRE_DOCUMENTO].html.

Por ejemplo:

- https://crispy-carnival-8f8f6875.pages.github.io/docs/proyecto1.html
- https://crispy-carnival-8f8f6875.pages.github.io/docs/proyecto2.html

## Documentos modernos con Material for Mkdocs (descripciones de proyectos, apuntes...)

Para hacer documentos, existe ahora una opción más completa usando [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/). Esto nos permite tener un framework personalizable y extendible, tal y como tenemos RevealJS para las diapositivas.

El origen del contenido sigue siendo Markdown, aunque es necesario configurar un poco más dependiendo de la navegación que prefieras dentro de la web que se genera. En la carpeta [mkdocs](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/main/mkdocs) hay dos proyectos de ejemplo, [apuntes1](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/main/mkdocs/apuntes1) y [apuntes2](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/main/mkdocs/apuntes2). Puedes copiarlos (o modificarlos) para crear los tuyos propios. Sólo debes modificar dentro de la carpeta el archivo **mkdocs.yml** para sustituir el nombre de apuntes1 o apuntes2 por el que hayas puesto a la carpeta de tu proyecto. El archivo base.yml de la carpeta mkdocs contiene la configuración que se va a aplicar a todos los proyectos por defecto.

Cada vez que se realiza una modificación en la carpeta mkdocs, se ejecutan dos Github Actions, [mkdocs-to-html](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/.github/workflows/mkdocs-to-html.yml) y [mkdocs-to-pdf](https://github.com/IES-Rafael-Alberti/uniform-documentation/blob/main/.github/workflows/mkdocs-to-pdf.yml). El primero genera una carpeta con todos los archivos del proyecto dentro de la carpeta docs. El segundo genera los archivos PDF de los proyectos dentro de la rama [exports](https://github.com/IES-Rafael-Alberti/uniform-documentation/tree/exports).

Si está activo [Github Pages](https://github.com/IES-Rafael-Alberti/uniform-documentation/settings/pages) en el repositorio, podrás acceder a la versión HTML de los proyectos simplemente escribiendo: [URL_GITHUB_PAGES_REPOSITORIO]/docs/[NOMBRE_PROYECTO].

Por ejemplo:

- https://crispy-carnival-8f8f6875.pages.github.io/docs/apuntes1
- https://crispy-carnival-8f8f6875.pages.github.io/docs/apuntes2

## ¿Y ahora qué?

Realiza un fork de este repositorio para tu módulo y comienza a escribir. Solamente queda que alguien bueno diseñando realice un CSS espectacular para estos archivos que se generan.
