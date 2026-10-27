# UD2.1 - Ejercicio 4: Identificadores y Atributos

## 1. Mensaje de error del Validador W3C (por duplicar id="corp")
Al introducir un segundo elemento con `id="corp"`, el validador oficial de W3C devuelve el siguiente error:
> **Error**: Duplicate ID `corp`.
> **From line X, column Y; to line Z, column W**
> *ID "corp" is already defined.*

## 2. ¿Por qué se desaconseja usar selectores de id para estilizar?
Se desaconseja el uso de selectores de `id` (`#`) en CSS por varios motivos:
1. **Especificidad excesiva:** Los identificadores tienen un peso de especificidad muy alto, lo que hace que sus reglas sean muy difíciles de sobrescribir o mantener a medida que el proyecto crece.
2. **Falta de reutilización:** Por definición, un `id` debe ser único en todo el documento HTML. No se puede aplicar el mismo estilo de `id` a varios elementos, mientras que las clases (`.clase`) están diseñadas precisamente para ser reutilizables.