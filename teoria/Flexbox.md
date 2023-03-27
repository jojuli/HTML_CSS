# :pencil: Flexbox 
* Es un modulo de maquetación que permite generar diseños atractivos para el usuario.
* Una guia interesante es [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

### :smile: Conceptos Básicos
 ![Estructura de Flexbox](https://github.com/jfisol/HTML_CSS/blob/main/teoria/img_flexbox/EstructuraFlexbox.jpg)

**Caracteristicas** :grin:
* Flexbox es un sistema unidimensional.
* El comportamiento del flexbox se le aplica a los elementos hijo.
* El tamaño del eje principal (cross axis)es definido por `x` (main size).
* El tamaño del eje secundario (cross size) es definido por `y`(cros axis).

### **[Propiedad contenedor padre](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-properties-for-the-parentflex-container)** :man:


  - Displey: `flex/inline-flex`
- Cuando se utiliza `flex` se definen en bloque los elementos padre.
- Cuando se utiliza inline-flex se definen el linea los elementos padre.

*Tener en cuenta que las columnas de css no tienen efecto en un contenedor flexible*

Ejemplo:
``.container  {  display: flex;  /* or inline-flex */  }``

***[Dirección de Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-flex-direction)*** :arrow_right:
Establece la dirección en la que se colocan los artículos flexibles (define el eje principal).
Ejemplo:
``.container  {  flex-direction: row | row-reverse | column | column-reverse;  } ``

***[Flex wrap](https://css-tricks.com/almanac/properties/f/flex-wrap/#aa-values)***

-   **`nowrap`(predeterminado):** una sola línea que puede hacer que el contenedor se desborde
-   **`wrap`:** multilíneas, la dirección está definida por`flex-direction`
-   **`wrap-reverse`:** multilíneas, opuestas a la dirección definida por`flex-direction`
Ejemplo:
``flex-wrap: nowrap | wrap | wrap-reverse``

    ***[Flex Flow](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-flex-flow)***
Esta es una forma abreviada de las propiedades `flex-direction`y `flex-wrap`, que juntas definen los ejes principal y transversal del contenedor flexible: forma prederminada es row nonwrap
Ejemplo:
``.container  {  flex-flow: column wrap;  }``

~~Nota:~~ ``box-sizing: border-box/inherit // permite que el borde de la caja comience desde el contenido``

***[Justify Contet](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-justify-content)***
**Esto define la alineación a lo largo del eje principal.**

Alinear el contenido, define la alineación de acuerdo al eje principal, ayuda a distribuir el espacio libre adicional sobrante cuando todos los elementos flexibles de una línea son inflexibles o son flexibles.
- en un estándar el eje (x).

![enter image description here](https://github.com/jfisol/HTML_CSS/blob/main/teoria/img_flexbox/justify_Content.png)

Ejemplo:
``.container  {  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ...  + safe | unsafe;  }``

***[Align items](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-align-items)***
**Esto define el comportamiento predeterminado de cómo se distribuyen los elementos flexibles a lo largo del ~~eje transversal~~ en la línea actual.**
- en un estándar el eje (y).

![enter image description here](https://github.com/jfisol/HTML_CSS/blob/main/teoria/img_flexbox/align_items.png)

Ejemplo:
``.container  {  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end +  ... safe | unsafe;  }``


