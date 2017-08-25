---
layout: post
published: true
title: Prueba de post desde prose.io
subtitle: E instrucciones para usar prose.io
date: '2017-08-25'
image: >-
  https://s3.amazonaws.com/kinlane-productions/api-evangelist/prose-io/prose-io-login.png
author: Carlos Cámara  
---
Este es un post escrito desde [prose.io](http://prose.io), un servicio que ofrece una interfaz para crear y editar posts de [jekyll](http://jekyllrb.com/) algo más amigable que editar archivos de markdown y subirlos a git, en la rama `gh-pages` para que se recompile el sitio web.

## Instrucciones:

1. Acceder a [prose.io](http://prose.io)
2. Identificarse con la cuenta de github
3. Buscar el repositorio `mapcolabora/mapcolabora-jekyll`
4. Hacer clic en crear nuevo post.
5. Escribir.
6. Previsualizar con el icono de la derecha.
7. Editar metadatos (en realidad está añadiendo campos al [front matter](https://jekyllrb.com/docs/frontmatter/) de los archivos markdown).
8. Darle a guardar.

## ¿Qué ha pasado tras las bambalinas?

Al crear un nuevo post ha creado un archivo en la carpeta `_posts` (en el caso de haber marcado la casilla `publish` de los metadatos) o en `_drafts`. En ambos casos el archivo sigue el siguiente patrón: `yyyy-mm-dd-título.md`

El archivo empieza con varios campos dentro de  `---` , eso es el front matter, y son los metadatos del post. Luego tiene el contenido que hayamos escrito.

Al guardarlo crea un nuevo commit (por eso vale la pena poner un mensaje molón) al repositorio y lo añade a la rama `gh-pages`. Si estaba marcado para publicar, esto es, en la carpeta `_posts`, aparecerá en la versión online de la web.

Github ejecuta jekyll y recompila el sitio, que es lo que se ve en la web.


## A New Post

Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.
