1. **static (`.c1` con `left: 50px`)**:
   - **¿Se mueve? ¿Por qué?** No se mueve en absoluto. El valor por defecto de los elementos es `static`, lo que significa que ignoran por completo propiedades de posicionamiento como `top`, `bottom`, `left` o `right`, respetando estrictamente el flujo normal de la página.

2. **relative (`.c2` con `top: 20px` y `left: 50px`)**:
   - Se desplaza visualmente desde su posición original. Sin embargo, **deja un hueco vacío** en el lugar donde debería estar, ya que el navegador sigue reservando su espacio físico original en el flujo del documento.

3. **absolute (`.c3` con `top: 0` y `right: 0`)**:
   - **¿A qué esquina va?** Sale del flujo normal de la página y se posiciona respecto al contenedor padre más cercano que tenga un posicionamiento distinto de `static` (en este caso, `.contenedor`). Va a la esquina superior derecha del contenedor.
   - **¿Qué pasa al añadir `position: relative` a `.contenedor`?** El cuadro absoluto toma como referencia exacta los límites de ese contenedor en lugar de la ventana del navegador. Los cuadros restantes ignoran por completo el hueco que ocupaba `c3` y ascienden como si este nunca hubiera estado allí.

4. **z-index y solapamiento (`.c1` y `.c2`)**:
   - Al desplazar `.c2` hacia arriba (`top: -40px`), este se solapa sobre `.c1`. Para conseguir que `.c1` vuelva a quedar por encima de `.c2`, se le aplica una propiedad de posicionamiento (diferente a `static`) junto con un `z-index` mayor (por ejemplo, `z-index: 2`), ya que el `z-index` **solo funciona en elementos posicionados**.