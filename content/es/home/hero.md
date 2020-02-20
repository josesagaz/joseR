+++
# Hero widget <- esto es un comentario.
widget = "hero"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true    # Activate this widget? true/false
weight = 10      # Order that this section will appear.

title = "Software Libre"

# Hero image (optional). Enter filename of an image in the `static/img/` folder.
hero_media = "AymaraTux.png"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"
  
  # Background gradient. #4bb4e3 end #2b94c3
  # gradient_start = "#536878"
  # gradient_end = "#aa3939"
  
  # Background image.
   image = "milky-way.jpg"  # Name of image in `static/img/`.
   image_darken = 0.4  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  # image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  # image_position = "center"  # Options include `left`, `center` (default), or `right`.
  # image_parallax = true  # Use a fun parallax-like fixed background effect? true/false
  
  # Text color (true=light or false=dark).
  text_color_light = true

# Call to action links (optional).
#   Display link(s) by specifying a URL and label below. Icon is optional for `[cta]`.
#   Remove a link/note by deleting a cta/note block.
[cta]
  url = "https://www.debian.org/distrib/"
  label = "Empezar aquí"
  icon_pack = "fas"
  icon = "arrow-alt-circle-down"
  
[cta_alt]
  url = "https://es.wikipedia.org/wiki/Software_libre"
  label = "Ver Documentación"

# Note. An optional note to show underneath the links.
[cta_note]
  label = '<a class="js-github-release"  href="https://www.debian.org/releases/stable/releasenotes">Última versión 10.3 (buster)</a>'
+++

Un software es libre si otorga a los usuarios de manera adecuada las denominadas cuatro libertades: **libertad de usar, estudiar, distribuir y mejorar,** de lo contrario no se trata de software libre. 