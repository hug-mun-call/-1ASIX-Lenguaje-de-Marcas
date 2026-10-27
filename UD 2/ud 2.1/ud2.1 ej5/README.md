# UD2.1 - Ejercicio 5: Detective de Colisiones y Refactorización

## Parte A — Análisis de Colisiones de Especificidad

| Elemento | Color Esperado / Real | Razón / Regla Ganadora |
| :--- | :--- | :--- |
| `<h1>` (`Hola CSS`) | **brown** (marrón) | El selector de ID (`#titulo`) gana a los selectores de clase (`.grande`) y de etiqueta (`h1`) por mayor especificidad. |
| `<p>` (`Texto 1`) | **purple** (púrpura) | `p.aviso` combina etiqueta y clase, lo que la hace más específica que `.aviso` (solo clase) o `p` (solo etiqueta). |
| `<p>` (`Texto 2`) | **black** (negro) | El selector de ID (`#importante`) tiene la mayor especificidad de todas las reglas aplicadas a este párrafo. |
| `<p>` (`Texto 3`) | **orange** (naranja) | El selector descendiente `div p` es más específico que los selectores simples de etiqueta `p`. |

### Explicación de la jerarquía de especificidad
1. **ID (`#`)**: Nivel más alto (peso: 1,0,0).
2. **Clase (`.`) y Atributos**: Nivel intermedio (peso: 0,1,0).
3. **Etiqueta/Elemento**: Nivel más bajo (peso: 0,0,1).
4. **Cascada**: A igual especificidad entre dos reglas, gana siempre la que se ha escrito en último lugar en el CSS.