# Visor Urbano Docs

En este repositorio se encuentra la documentación del proyecto Visor Urbano.

Para correr este repositorio necesitas:

- Ruby ~>3.0
- Bundler ~2.5.9
- [Jekyll] ~4.3.4

Este sitio utiliza la plantilla [Just the Docs] para su tema.

## Correr y previsualizar el sitio localmente

Asumiendo que [Jekyll] y [Bundler] están instalados en tu computadora:

1.  Cambia tu directorio al directorio raíz de este sitio.

2.  En la terminal corre `bundle install`.

3.  Después corre `bundle exec jekyll serve --watch --livereload` para compilar y previsualizar el sitio en `localhost:4000`.

    El sitio compilado estará disponible en la carpeta `_site`.


## Publicar el sitio en GitHub Pages

1.  Si tu sitio creado está en `YOUR-USERNAME/YOUR-SITE-NAME`, actualiza el archivo `_config.yml` a:

    ```yaml
    title: YOUR TITLE
    description: YOUR DESCRIPTION
    theme: just-the-docs

    url: https://YOUR-USERNAME.github.io/YOUR-SITE-NAME

    aux_links: # remove if you don't want this link to appear on your pages
      Template Repository: https://github.com/YOUR-USERNAME/YOUR-SITE-NAME
    ```

2.  Empuja tus cambios al `_config.yml` de tu Github.

3.  En tu repositorio de GitHub:
    - Ve a la pestaña `Settings` opción -> `Pages` -> `Build and deployment`, y selecciona `Source`: `GitHub Actions`.
    - Si alguna de las Actions falló, ve a `Actions` y da click en `Re-run jobs`.

## Publicar el sitio en una plataforma distinta

Sólo sube todos los archivos compilados en la carpeta `_site`.

## Alojar la documentación en un repositorio existente

Si quieres desplegar esta documentación desde un repositorio existente, puedes compiar los archivos de este repositorio en el fólder `docs` y modificar el workflow de Github Actions para construir desde el directorio `docs`. 

## Licensing and Attribution

This repository is licensed under the [MIT License]. You are generally free to reuse or extend upon this code as you see fit; just include the original copy of the license (which is preserved when you "make a template"). While it's not necessary, we'd love to hear from you if you do use this template, and how we can improve it for future use!

The deployment GitHub Actions workflow is heavily based on GitHub's mixed-party [starter workflows]. A copy of their MIT License is available in [actions/starter-workflows].

----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Jekyll]: https://jekyllrb.com
[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[Bundler]: https://bundler.io
[MIT License]: https://en.wikipedia.org/wiki/MIT_License
