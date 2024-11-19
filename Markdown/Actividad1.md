**Paso 1: Preparación del entorno**

1. - Empiezo asegurándome de que tengo Ruby y Bundler instalados en mi sistema local. Para verificarlo, ejecuto:
```
bash

Copiar código

ruby -v

bundler -v
```
Si no están instalados, los instalo con:
```
bash

Copiar código

sudo apt install ruby-full

gem install bundler
```

**Paso 2: Instalación de Jekyll**

1. - Instalo Jekyll utilizando Bundler:
```
bash

Copiar código

gem install jekyll
```
1. - Creo un nuevo sitio de Jekyll llamado *mi-blog*:
```
bash

Copiar código

jekyll new mi-blog

cd mi-blog
```
**Paso 3: Configuración inicial**

1. - Abro el archivo \_config.yml en mi editor de texto preferido (por ejemplo, nano o vim) y personalizo los valores:

yml
```
title: "Mi Blog Personal"

author: 

`  `name: "Rodrigo Gonzalez"

email: "rgonzalezc14@educantabria.es"

description: "Un blog sobre mi."
```
1. - Guardo y cierro el archivo.

**Paso 4: Ejecuto el servidor local**

1. - Inicio el servidor local de Jekyll para previsualizar mi sitio:

bash

Copiar código

bundle exec jekyll serve

1. - Accedo a http://localhost:4000 en mi navegador para ver mi sitio.

**Paso 5: Personalización de las páginas**

1. - Edito la página principal index.markdown con contenido que describa el propósito del blog.

markdown

Copiar código
```
\---

layout: page

title: "Contacto"

permalink: /contacto/

\---
```

**Paso 6: Creación de publicaciones (posts)**

1. Creo al menos 3 publicaciones en la carpeta \_posts con nombres que sigan el formato YYYY-MM-DD-titulo.md:

markdown

Copio el código

```

layout: post

title: "Mi Primera Publicación"

date: 2024-11-08

```

Aquí describo la primera entrada de mi blog sobre la temática seleccionada.

**Paso 7: Configuración de GitHub Pages**

1. - Creo un nuevo repositorio en GitHub llamado *mi-blog*.
2. - En mi terminal, inicializo un repositorio Git en el directorio local y lo vinculo a GitHub:
```
bash

Copiar código

git init

git remote add origin https://github.com/RodrigoGColl/miblog.git
```

1. - Agrego todos los archivos, realizo el primer commit y subo el contenido:

```
Copiar código

git add .

git commit -m "Primer commit del blog"

git branch -M main

git push -u origin main

```

**Paso 8: Configuración de GitHub Pages**

1. - En GitHub, voy a la configuración del repositorio (*Settings*), busco la sección *Pages* y selecciono la rama main en la carpeta raíz (/).
1. - Guardo los cambios y espero a que GitHub Pages despliegue el sitio.