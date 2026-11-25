# Actividad: Web responsive con media queries - Club de Senderismo Monte Verde

## Ejercicio 1. Diagnóstico inicial (sobre el código base)

Al inspeccionar la versión previa en modo dispositivo a **360 px** y **768 px**, se detectan los siguientes problemas:

1. **Contenedor principal (`.contenedor`)**: A 360 px y 768 px aparece una barra de desplazamiento horizontal porque el contenedor tiene un ancho fijo (`width: 960px`) que supera el ancho de ambas pantallas.
2. **Sello circular (`.sello`)**: A 360 px el sello de 84 px posicionado de forma absoluta en la esquina superior derecha invade el espacio del título `<h1>` y se solapa con el texto.
3. **Menú de navegación (`nav`)**: A 360 px los enlaces están en línea (`inline-block`) y se quedan fijos arriba (`sticky`), ocupando demasiada altura si saltan de línea o quedando demasiado estrechos para pulsar cómodamente en móvil.
4. **Tarjetas de rutas (`.tarjeta`)**: Tienen un ancho fijo de `270px` y márgenes laterales, por lo que en 360 px sobra mucho espacio vacío a los lados en lugar de ocupar el ancho disponible, y a 768 px la segunda tarjeta sigue elevada (`top: -12px`) rompiendo la alineación si se colocan en dos filas.
5. **Galería de polaroids (`.galeria-contenedor` y `.polaroid`)**: A 360 px y 768 px las fotos se salen completamente de la pantalla por la derecha porque tienen posicionamiento absoluto con coordenadas fijas (`left: 290px` y `left: 500px`) pensadas solo para 960 px.

## Ejercicio 4. Pruebas y capturas

- ![Vista móvil 360px](se llama captura-360.png)
- ![Vista escritorio 1200px](se llama captura-1200.png)