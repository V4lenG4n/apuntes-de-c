# 01 — Introducción y Estructura

Todo programa en C tiene esta forma mínima:

```c
// 1. Incluir librería de entrada/salida
#include <stdio.h>

// 2. Función principal — punto de entrada del programa
int main() {

    // 3. Instrucción que imprime en pantalla
    printf("Hola, Mundo!\n");

    // 4. Retorna 0 = éxito al sistema operativo
    return 0;
}
```

## Componentes principales

| Componente | Qué hace |
|---|---|
| `#include <stdio.h>` | Importa funciones de entrada/salida (printf, scanf...) |
| `int main()` | Función obligatoria — el programa arranca aquí |
| `{ ... }` | Bloque de código de la función |
| `;` | Toda instrucción termina con punto y coma |
| `return 0;` | Indica que el programa terminó sin errores |
| `// comentario` | Comentario de una línea (el compilador lo ignora) |
| `/* ... */` | Comentario de varias líneas |

---


