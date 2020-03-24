blogdown::new_site(theme="gcushen/hugo-academic")

### para ver en tiempo real los cambios.
blogdown::serve_site()

### in Rstudio seria toolbar -> Addins -> Serve Site

### ahora solo es editar, CRUDE (Crear Update 'actualizar' Delete 'borrar' Editar)

### a veces se necesita reconstruir la pagina web
blogdown::hugo_build()

# Personalizar
## se necesita conocer estos lugares

1. _config.toml_
2. _content/_ es la carpeta donde van los documentos que creamos
3. _Public/_ la carpeta donde R genera el sitio web
4. _static_ carpeta done estan las imagenes.

> * editar config.toml (ahi va tu email, twitter etc.)
  * Se puede editar el contenido de _content_ y _static_ directamente!
  * Tambien puedes usar el **Addins** de la barra de heramientas para crear nuevos posts y agregar imagenes.

# Crear nuevo post(s)
#### toolbar -> Addins -> New Post
> dejo 1:44

# Mapa de los módulos en la primera página

: Tabla1 Orden de los módulos y su equivalente

| Modulo en Ingles | cambio en castellano  |
|-----------------:|:---------------------:|
|             hero | porque SL             |
|            about | Movimiento del SL     |
|             demo | Debian - El SO Univer |
|           skills | Objetivos  *          |
|       experience | Trajectoria  *        |
|            posts | Artículos             |
|         projects | Proyectos             |
|            talks | Galería               |
|         featured | Talleres de F         |
|     publications | Featured Publications |
|             tags | Recent Publications   |
|          contact | Contact               |
|                  |                       |
(*) estan apagados esto widgets --> active = false 


:Tabla2 El Menu principal y donde enlaza.

|          Menú | Módulo de enlace |
|--------------:|:----------------:|
|        Inicio | hero             |
|     Artículos | posts            |
|     Proyectos | projects         |
| Publicaciones | publications     |
|        Cursos | /courses/index   |
|      Contacto | contact          |
|               |                  |



# La licencia de GPLv3
https://lslspanish.github.io/translation_GPLv3_to_spanish/

# Para añadir Disqus a Hugo template
https://notes.peter-baumgartner.net/tutorial/how-to-install-disqus-on-hugo/

# listado de iconos emoji 
https://gist.github.com/rxaviers/7360908
