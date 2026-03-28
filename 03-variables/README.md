# 03 — Variables y Constantes

## Variables

Una variable es un espacio en memoria con un nombre, un tipo y un valor que puede cambiar.

```c
// tipo   nombre     = valor inicial;
int    edad        = 20;
float  precio      = 10.99;
double distancia   = 12345.6789;
char   letra       = 'A';      // comillas simples para char
```

## Tipos de datos básicos

| Tipo | Qué guarda | Tamaño | Ejemplo |
|---|---|---|---|
| `int` | Enteros | 4 bytes | `int x = 10;` |
| `float` | Decimales simples | 4 bytes | `float f = 3.14;` |
| `double` | Decimales doble precisión | 8 bytes | `double d = 1.23;` |
| `char` | Un carácter | 1 byte | `char c = 'A';` |

## Constantes

```c
// Con const — el compilador verifica que no se modifique
const float PI = 3.1416;
PI = 4.0;  // ❌ ERROR en compilación

// Con #define — reemplaza el texto antes de compilar
#define MAX 100
```

| | `const` | `#define` |
|---|---|---|
| Ocupa memoria | Sí | No |
| Tiene tipo | Sí | No |
| El compilador la verifica | Sí | No |

## Reglas para nombres de variables

- Empezar con letra o `_`
- Sin espacios
- Sin palabras reservadas (`int`, `if`, `while`...)
- Sensible a mayúsculas (`edad` ≠ `Edad`)

---


