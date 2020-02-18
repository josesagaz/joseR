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

> editar config.toml (ahi va tu email, twitter etc.)
se puede editar el contenido de _content_ y _static_ directamente!
tambien puedes usar el **Addins** de la barra de heramientas para crear nuevos posts y agregar imagenes.

# Crear nuevo post(s)
#### toolbar -> Addins -> New Post
> dejo 1:44

---
