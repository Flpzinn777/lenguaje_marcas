Inline-block y display: flex:
Lo prefiero porque es mucho más cómodo. Con inline-block me pasó que la tercera tarjeta saltaba de línea por culpa del espacio en blanco que hay entre los div en el HTML, y eso me obligó a ir ajustando medidas. Con flex ese problema desaparece y las tres tarjetas quedan en fila sin tocar nada más.

¿Qué diferencia hay entre margin y padding?
El padding es el espacio interior, entre el contenido y el borde, y lleva el color de fondo. El margin es el espacio exterior, fuera del borde, y siempre es transparente

¿Por qué saltaba la tercera tarjeta de línea?
Porque cada tarjeta ocupa más que su width
220 + 30 (padding) + 2 (borde) + 20 (margin) = 272px
Tres tarjetas suman 816px, pero dentro de .pagina solo hay unos 756px disponibles, haciendo con que la tercera tarjeta se baje sola


¿Qué propiedades ignoraba el <span> y por qué?
Ignoraba width, height y los márgenes verticales, porque un <span> es display: inline y se comporta como una palabra dentro del texto: no admite dimensiones propias. Con inline-block sí se aplican

Qué hace display: none con el espacio que ocupaba la caja?
Lo elimina por completo: el elemento no se ve ni ocupa sitio, así que no queda hueco y las demás tarjetas ocupan su lugar