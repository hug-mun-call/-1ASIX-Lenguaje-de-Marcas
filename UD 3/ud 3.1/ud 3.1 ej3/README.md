## Respuestas y observaciones del ejercicio:

### Parte A — Tarjeta de producto
1. **¿Qué elemento necesita `position: relative` para que la etiqueta se coloque respecto a la tarjeta?**
   - El contenedor principal de la tarjeta (`.tarjeta-producto`) es el que debe llevar `position: relative`. De esta manera, al asignarle `position: absolute` a la etiqueta de descuento, esta toma como referencia los límites de la tarjeta en lugar de la ventana del navegador.
2. **¿Qué le pasa a la parte de la etiqueta que sobresale al poner `overflow: hidden`?**
   - Al activar `overflow: hidden`, la parte de la etiqueta que sobresale fuera de los bordes de la tarjeta **se corta y desaparece visualmente**. Esto ocurre porque `overflow: hidden` recorta todo el contenido que desborda los límites de la caja contenedora. Para arreglarlo y permitir que sobresalga decorativamente, se debe eliminar o no aplicar dicho `overflow` en el contenedor principal de la tarjeta.

### Parte B — Caja de comentarios y propiedades de desbordamiento
1. **Diferencias entre los valores de `overflow` probados:**
   - **`visible`**: Es el valor por defecto. El contenido que no cabe se sale de los límites de la caja y se muestra por encima de los elementos de debajo.
   - **`hidden`**: El contenido sobrante se oculta y no se puede ver ni alcanzar mediante desplazamiento.
   - **`scroll`**: Muestra barras de desplazamiento (tanto horizontal como vertical) de forma permanente, independientemente de si el contenido cabe o no.
   - **`auto`**: Muestra las barras de desplazamiento **solo cuando es necesario** (cuando el contenido sobrepasa las dimensiones de la caja). Es el comportamiento más limpio y recomendado.

2. **Diferencia entre `visibility: hidden` y `display: none`:**
   - **`visibility: hidden`**: Oculta el elemento visualmente, pero **deja intacto el espacio físico** que ocupaba en la página (queda un hueco en blanco).
   - **`display: none`**: Elimina el elemento por completo del flujo del documento, haciendo que **desaparezca y no deje ningún hueco**, permitiendo que los elementos adyacentes ocupen su lugar.