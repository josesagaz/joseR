# Blogdown

Blogdown es un paquete desarrollado por _Yihui Xie_, creador de **knitr, bookdown** y un nuevo paquete de diapositivas **xaringan**

Te permite crear bonitos sitios web y publicar blogs usando **R Markdown**

---

Un recurso disponible es el libro  [blogdown: Creating Websites with R Markdown](https://bookdown.org/yihui/blogdown/) está completo y es gratis cortesía del autor: _Xie, Thomas y Hill (2018_).

Blogdown crea y construye el sitio web a partir de documentos (R) Markdown (¡no solo para blogs!)

---

Como cada página es un archivo .Rmd (o .Md), ¡también puedes publicar tus materiales como documentos portátiles!

Hereda muchas características de **bookdown** (_Xie, 2016_), incluido el formateo de **LaTeX** y las citas de **BibTeX.**


{{< speaker_note >}}
- Only the speaker can read these notes
- Press `S` key to view
{{< /speaker_note >}}


---

## Panorama general

1. Instalar Blogdown y Hugo

2. Crear nuevo sitio

3. Crear una cuenta de Netlify (o updog, páginas de GitHub, etc.)

4. Crear el contenido (por ejemplo, nuevas publicaciones)

---

5. Implementar el sitio a través de Netlify con (o sin) GitHub

6. Repita los pasos 4-6 según sea necesario.

Necesitaras...

* Crear un nuevo proyecto en R Studio:

        install.packages ("blogdown")

        blogdown::install_hugo

---

* Crear nuevo sitio:

        blogdown::new_site()

* ¡Este comando generará la estructura de tus directorios y archivos de tu sitio web!

* Pon tu sitio web en un repositorio de GitHub (recomendado)
* Implementar tu sitio web a través de Netlify.com

---

También se puede alojar el sitio web en GitHub: con el nombre del repositorio de tu sitio web _username.github.io_

Si deseas esto, consulta el tutorial de [Amber Thomas:](http://amber.rbind.io/blog/2016/12/19/creatingsite/)

Si tienes un dominio registrado (por ejemplo, yourname.com), ¡puedes usarlo en su lugar!

---

### Otros Recursos

¡Puedes migrar desde jekyll, wordpress, blogger, etc.!

[El libro oficial de Blogdown](https://bookdown.org/yihui/blogdown/)

[Gran paso a paso de Allison Presmanes Hill](https://alison.rbind.io/post/up-and-running-with-blogdown/)

[Tutorial mencionado anteriormente por Amber Thomas](http://amber.rbind.io/blog/2016/12/19/creatingsite/)

---

# ¿qué es Hugo?

Hugo es un generador de sitio estático gratuito y de código abierto (como Jekyll)

¡Probablemente quieras elegir una plantilla! 

* https://themes.gohugo.io/
* plantillas accesibles como repositorios github

       blogdown::new_site(theme = "user/repo", theme_example = TRUE)

---

* Usaremos la plantilla _"gcushen/hugo-academic"_
* ¡Usar la plantilla con la configuración predeterminada

---

# Construir y personalizar el sitio web

---

## Construir:

```
blogdown::new_site(theme="gcushen/hugo-academic")

### ver los cambios en tiempo real del sitio en R Studio; 
### sitio de auto-construcción con cada cambio!

blogdown::serve_site() 

### o barra de herramientas -> Addins -> Serve site
### ahora editar el sitio, crear nuevas publicaciones y 
### guardar los archivos cuando termine:
### ¡su sitio se actualizará automáticamente!
### alternativamente, explícitamente reconstruir el sitio a través de

blogdown::hugo_build ()
```
---

# Personalizar

### se necesita conocer estos lugares

1. _config.toml_
2. _content/_ es la carpeta donde van los documentos que creamos

---

3. _Public/_ la carpeta donde R genera el sitio web
4. _static/_ carpeta done estan las imagenes.

> * editar config.toml (ahi va tu email, twitter etc.)
> * Se puede editar el contenido de _content/_ y _static/_ directamente!
> * Puedes usar el **Addins** de la barra de heramientas para crear nuevos posts y agregar imagenes.

---

# Crear nuevo post
#### toolbar -> Addins -> New Post

* Ingrese: Título, Autor, y otros metadatos
* Grabarlo como: .Rmd ó .Md
* Use el marcado de Markdown para la composición de los documentos
* Puede insertar imágenes con Addins -> Insert Image

---

# GitHub

*  En la cuenta de GitHub, crear un nuevo repositorio (con el nombre del sitio pudes ser cualquier nombre)
* No inicializar con Readme, license, or gitignore (se hara eso mas tarde)
* Hacer click a "clone or download" y copie el enlace.

---

* en la terminal hacer _cd_ al directorio donde se encuentra su proyecto de R

```
git init
git add .
git commit -m "primera version de mi sitio web"
git remote add origin REMOTE_REPO_URL <- ahí va el enlace que copiamos de GitHub
git push -u origin master
```
---

# Netlify.com

* ¡Implementación gratuita de sitios web estáticos!

---

* ¡Fácil de usar! ¡Personalización de nombre de dominio gratis!
  + Regístrese con una cuenta existente de GitHub
  + Inicie sesión y seleccione "nuevo sitio de Git"
  + Navegue al repositorio de su sitio web
  + En "Basic build settings" ... Comando de compilación: hugo_0.20, Publish directory: public

---

* _Nota:_ si usa un template complejo, es posible que necesite el comando Build hugo, y luego desplácese hacia abajo para construir variables de entorno y coloque HUGO_VERSION y 0.40 (o cualquier versión que tenga; escriba ```hugo version``` en la línea de comandod).
