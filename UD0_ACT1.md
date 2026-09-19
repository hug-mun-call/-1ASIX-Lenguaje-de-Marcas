# ACTIVIDAD 1
Mi conclusión es que al principio cuando lo abro no queda igual, el .txt muestra el código literal sin procesar y el .html procesa las etiquetas y aplica lo que le he pedido.

# Actividad 2
```
<dam>
<modulo><titulo>Lenguaje de Marcas</titulo>
<contenido>
<unidad>Introducción</unidad>
<unidad>HTML</unidad>
<unidad>CSS</unidad>
</contenido>
</modulo>
<modulo><titulo>Base de datos</titulo>
<contenido>
<unidad>Introducción</unidad>
<unidad>Edición de datos</unidad>
<unidad>Realización de consultas</unidad>
</contenido>
</modulo>
<modulo><titulo>Lectura y escritura de información</titulo>
<contenido>
<unidad>Introducción</unidad>
<unidad>Flujos de entrada y salida</unidad>
<unidad>Manejo de archivos de texto y binarios</unidad>
</contenido>
</modulo>
</dam>
```
# Actividad 3
```
<!DOCTYPE paises [
  <!ELEMENT paises - - (pais+)>
  <!ELEMENT pais - - (nombre, capital, continente, poblacion, moneda)>
  <!ELEMENT nombre - - (#PCDATA)>
  <!ELEMENT capital - - (#PCDATA)>
  <!ELEMENT continente - - (#PCDATA)>
  <!ELEMENT poblacion - - (#PCDATA)>
  <!ELEMENT moneda - - (#PCDATA)>
]>

<paises>

  <pais>
    <nombre>Espana</nombre>
    <capital>Madrid</capital>
    <continente>Europa</continente>
    <poblacion>47000000</poblacion>
    <moneda>Euro</moneda>
  </pais>

  <pais>
    <nombre>Japon</nombre>
    <capital>Tokio</capital>
    <continente>Asia</continente>
    <poblacion>125000000</poblacion>
    <moneda>Yen</moneda>
  </pais>

  <pais>
    <nombre>Brasil</nombre>
    <capital>Brasilia</capital>
    <continente>America del Sur</continente>
    <poblacion>214000000</poblacion>
    <moneda>Real</moneda>
  </pais>

</paises>
```
