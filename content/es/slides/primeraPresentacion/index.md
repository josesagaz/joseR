---
authors: [José SagaZ]
categories: []
date: "2019-02-05T00:00:00Z"
slides:
  highlight_style: dracula
  theme: league  
  #  black: Black background, white text, blue links (default theme)
  #  white: White background, black text, blue links
  #  league: Gray background, white text, blue links (default theme for reveal.js < 3.0.0)
  #  beige: Beige background, dark text, brown links
  #  sky: Blue background, thin dark text, blue links
  #  night: Black background, thick white text, orange links
  #  serif: Cappuccino background, gray text, brown links
  #  simple: White background, black text, blue links
  #  solarized: Cream-colored background, dark green text, blue links

summary: Una introducción al uso de la función de diapositivas en la plantilla Academic.
tags: []
title: Slides-pepito
---

# Crear diapositivas con Markdown en Academic

[Academic](https://sourcethemes.com/academic/) | [Documentación](https://sourcethemes.com/academic/docs/managing-content/#create-slides)

---

## Características

- Escriba diapositivas de manera eficiente en Markdown
- 3 en 1: cree, presente y publique sus diapositivas
- Contiene notas del orador
- Diapositivas amigables para dispositivos móviles

---

## Controles

- Siguiente: `Flecha derecha` o` Espacio`
- Anterior: `Flecha izquierda`
- Inicio: `Inicio`
- Terminar: `Fin`
- Descripción general: `Esc`
- Notas del orador: `S`
- Pantalla completa: `F`
- Zoom: `Alt + Click`
- [Exportar PDF] (https://github.com/hakimel/reveal.js#pdf-export): `E`

---

## Resaltado de código

Código en línea: `variable`

Bloque de código:
```pitón
capuccino = "cafe"
if capuccino == "cafe":
     print ("Tomar ...")
```

---

## Matemáticas

Matemáticas en línea: $ x + y = z $

Bloque matemático:
$$
f\left( x \right) = \;\frac{{2\left( {x + 4} \right)\left( {x - 4} \right)}}{{\left( {x + 4} \right)\left( {x + 1} \right)}}
$$

---

## Fragmentos

Hacer que el contenido aparezca incrementalmente
```
{{%/* fragment */%}} Uno {{%/* /fragment */%}}
{{%/* fragment */%}} **Dos** {{%/* /fragment */%}}
{{%/* fragment */%}} Tres {{%/* /fragment */%}}
```

¡Presiona `Espacio` para iniciar  !


{{% fragment %}} Uno {{% /fragment %}}
{{% fragment %}} **Dos** {{% /fragment %}}
{{% fragment %}} Tres {{% /fragment %}}

---

Un fragmento puede aceptar dos parámetros opcionales:

- `class`: usa un estilo personalizado (requiere definición en CSS personalizado)
- `weight`: establece el orden en que aparece un fragmento

---

## Notas del presentador

Agregue sus notas de su presentación

```markdown
{{%/* speaker_note */%}}
- Solo el presentador puede leer estas notas
- Presione la tecla `S` para ver
{{%/* /speaker_note */%}}
```

¡Presione la tecla `S` para ver las notas del orador!

{{<speaker_note>}}
- Solo el presentador puede leer estas notas
- Presione la tecla `S` para ver
{{</speaker_note>}}

---

## Temas (conjunto de tonalidades)

- black: Fondo negro, texto blanco, enlaces azul (por defecto)
- white: Fondo blanco, texto negro, enlaces azul 
- league: Fondo gris, texto blanco, enlaces azul
- beige: Fondo beige, texto obscuro, enlaces marron
- sky: Fondo azul, texto obscuro, enlaces azul 

---

- night: Fondo negro, texto blanco gureso, enlaces naranja 
- serif: Fondo cafe, texto gris, enlaces marron 
- simple: Fondo blanco, texto negro, enlaces azul
- solarized: Fondo crema, texto verde obscuro, enlaces azul 

---

{{< slide background-image="/img/boards.jpg" >}}

## Diapositiva personalizada

Personaliza el estilo y el fondo de la diapositiva asi:

```markdown
{{</* slide background-image="/img/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

# Ejemplo de CSS personalizado

Hagamos encabezados de color azul marino.

Crea `assets/css/revel_custom.css` con:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# ¿Preguntas?

[Preguntas](https://spectrum.chat/academic)

[Documentación](https://sourcethemes.com/academic/docs/managing-content/#create-slides)
