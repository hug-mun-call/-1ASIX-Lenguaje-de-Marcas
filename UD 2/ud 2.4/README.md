
1. **¿Qué diferencia hay entre margin y padding?**
   - El **padding** es el espacio interior que hay entre el contenido de la caja y su borde.
   - El **margin** es el espacio exterior que separa una caja de los elementos que tiene alrededor.

2. **¿Por qué saltaba la tercera tarjeta de línea al usar inline-block?**
   - Saltaba porque las cajas de tipo `inline-block` suman sus anchos, los márgenes, los bordes y además respetan los espacios en blanco (saltos de línea) del código HTML entre etiqueta y etiqueta. Al sobrepasar el ancho disponible del contenedor (800px), el navegador obligaba a la tercera tarjeta a pasar a la siguiente línea. Usando `display: flex` en el contenedor se soluciona de forma más limpia.

3. **¿Qué propiedades ignoraba el <span> y por qué?**
   - El elemento `span` es un elemento en línea (`display: inline`). Por defecto, los elementos en línea ignoran las propiedades de ancho (`width`), alto (`height`) y los márgenes verticales (`margin-top` / `margin-bottom`). Al cambiarlo a `display: inline-block`, pasó a comportarse como una caja y ya sí respetó esas medidas.

4. **¿Qué hace display: none con el espacio que ocupaba la caja?**
   - `display: none` hace que el elemento desaparezca por completo de la pantalla y, a diferencia de `visibility: hidden`, **elimina el espacio que ocupaba**, haciendo que las demás cajas vecinas reconquisten ese hueco y se reajusten automáticamente.