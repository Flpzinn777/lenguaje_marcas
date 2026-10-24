¿Qué elemento necesita position: relative para que la etiqueta se coloque respecto a la tarjeta?
postion: absolute, asi tenemos el "control total" de este div dentro del div padre

¿Qué le pasa a la parte de la etiqueta que sobresale? 
con overflow: hidden todo lo que sobrepasa del div que tiene este argumento se elimina

Comentario:
Overflow
visible: es el valor por defecto. No corta nada, así que los comentarios que no caben se salen de la caja y se pintan encima de lo que  
haya debajo.
hidden: corta lo que no cabe y no deja ninguna forma de verlo, no hay barra de scroll.
scroll: corta lo que no cabe y siempre muestra las barras de scroll, aunque no hagan falta.
auto: igual que scroll, pero la barra solo aparece cuando el contenido no cabe.

Con visibility: hidden la tarjeta no se ve, pero sigue ocupando su sitio, Con display: none la tarjeta 
desaparece del todo y no deja hueco