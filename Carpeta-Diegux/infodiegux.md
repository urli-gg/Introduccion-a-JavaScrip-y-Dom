## Alcance de Variables y Funciones en JavaScript

### Tipos de Alcance (Scope)

- **Alcance global:** Variables declaradas fuera de cualquier función o bloque, accesibles desde cualquier lugar.
- **Alcance local (de función):** Variables declaradas dentro de funciones, accesibles sólo dentro de ellas.
- **Alcance de bloque:** Variables declaradas con `let` o `const` dentro de un bloque `{}`, solo existen en ese bloque.

### Declaraciones y Alcance

| Declaración | Alcance | Características                                       |
| ----------- | ------- | ----------------------------------------------------- |
| `var`       | Función | No respeta el alcance de bloque, se eleva (hoisting). |
| `let`       | Bloque  | Respeta el alcance de bloque, no se eleva.            |
| `const`     | Bloque  | Como `let`, pero el valor no puede reasignarse.       |

### Alcance de Funciones

- Las funciones tienen alcance léxico, es decir, pueden acceder a las variables del entorno donde fueron creadas (cadena de alcance).
- Variables y funciones locales no son accesibles desde el exterior.

---

## Tipos de Operadores en JavaScript

### Operadores Aritméticos

| Operador | Descripción                          | Ejemplo   |
| -------- | ------------------------------------ | --------- |
| `+`      | Suma                                 | `6 + 9`   |
| `-`      | Resta                                | `20 - 15` |
| `*`      | Multiplicación                       | `3 * 7`   |
| `/`      | División                             | `10 / 5`  |
| `%`      | Módulo (residuo de una división)     | `8 % 3`   |
| `**`     | Exponenciación                       | `2 ** 3`  |
| `++`     | Incremento unario                    | `x++`     |
| `--`     | Decremento unario                    | `x--`     |
| `+`      | Positivo unario (convierte a número) | `+"3"`    |
| `-`      | Negación unaria                      | `-x`      |

### Operadores de Asignación

| Operador | Función                 | Ejemplo   |
| -------- | ----------------------- | --------- |
| `=`      | Asignación simple       | `x = 3`   |
| `+=`     | Suma y asigna           | `x += 4`  |
| `-=`     | Resta y asigna          | `x -= 3`  |
| `*=`     | Multiplica y asigna     | `x *= 3`  |
| `/=`     | Divide y asigna         | `x /= 5`  |
| `%=`     | Módulo y asigna         | `x %= 2`  |
| `**=`    | Exponenciación y asigna | `x **= 2` |

### Operadores de Comparación

| Operador | Función                            | Ejemplo   |
| -------- | ---------------------------------- | --------- |
| `==`     | Igualdad (con conversión)          | `x == y`  |
| `===`    | Igualdad estricta (sin conversión) | `x === y` |
| `!=`     | Diferente                          | `x != y`  |
| `!==`    | Diferente estricta                 | `x !== y` |
| `>`      | Mayor que                          | `x > y`   |
| `<`      | Menor que                          | `x < y`   |
| `>=`     | Mayor o igual                      | `x >= y`  |
| `<=`     | Menor o igual                      | `x <= y`  |

### Operadores Lógicos

| Operador | Función               | Ejemplo  |
| -------- | --------------------- | -------- | ------------- | --- | --- | --- |
| `&&`     | AND lógico (y)        | `x && y` |
| `        |                       | `        | OR lógico (o) | `x  |     | y`  |
| `!`      | NOT lógico (negación) | `!x`     |

---

[INFO DE LA IA](https://www.perplexity.ai/search/me-puedes-dar-informacion-de-a-DFzzzFS8R6SnHHUh7Ssxfw#0)
