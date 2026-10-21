1. static
¿Se mueve? ¿Por qué?
El valor por defecto de los elementos "static", las propiedades de desplazamiento no tienen ningún efecto en ellas, ya que estos respetan estrictamente el flujo normal del documento

2. relative
¿Qué pasa con el hueco que deja?
El cuadro c2 se desplaza visualmente de su posición original, pero su hueco original permanece intacto en el flujo del documento. Los demas elementos actúan como si c2 siguiera exactamente en su sitio, por lo que no se mueven para ocupar el espacio libre que deja

3. absolute
¿A qué esquina va?
Si .contenedor no tiene ningún posicionamiento explícito, c3 se sale del contenedor y va a la esquina superior 
derecha de la ventana del navegador.

Ahora añade position: relative a .contenedor. ¿Qué cambia?
c3 se desplaza y se coloca exactamente en la esquina superior derecha de .contenedor

¿Qué hacen los demás cuadros con el hueco de c3?
Como position en absolute saca al elemento del flujo normal del documento, el hueco que ocupaba c3 desaparece por completo. Los demas elementos y el texto de debajo ignoran su existencia previa y reorganizan sus posiciones para rellenar ese espacio.

4. z-index
¿Cómo conseguir que c1 quede por encima de c2 usando z-index?
Ambos cuadros hay que estar en position relative, ya que z-index no funciona en elementos con pesition: static. y asegurar que el valor de c1 sea superior que el de c2