# 08 — Casting (Conversión de Tipos)

El **casting** es convertir un valor de un tipo a otro. Hay dos formas: implícita (automática) y explícita (manual).

## Implícita — el compilador convierte solo

```c
int   a = 5;
float b = a;    // int → float automáticamente (b = 5.0)
```

## Explícita — vos forzás la conversión

Se escribe el tipo deseado entre paréntesis antes del valor.

```c
int   x = 7;
int   y = 2;
float resultado = (float) x / y;  // → 3.5
// Sin el cast: 7 / 2 = 3 (división entera, pierde decimales)
```

## Ejemplos comunes

```c
int   entero  = (int) 3.99;    // → 3   (trunca, no redondea)
float decimal = (float) 5;     // → 5.0
char  letra   = (char) 65;     // → 'A' (valor ASCII)
int   codigo  = (int) 'A';     // → 65  (código ASCII)
```

## Tabla de conversiones

| Conversión | Resultado | Nota |
|---|---|---|
| `int` → `float` | `5` → `5.0` | No pierde información |
| `float` → `int` | `3.99` → `3` | Trunca (no redondea) |
| `int` → `char` | `65` → `'A'` | Usa tabla ASCII |
| `char` → `int` | `'A'` → `65` | Devuelve el código ASCII |
| `int / int` | `7 / 2` → `3` | División entera, pierde decimales |
| `(float) int / int` | `7 / 2` → `3.5` | Con cast recupera los decimales |

## Error típico — división entera

```c
int total    = 10;
int cantidad = 3;

float mal  = total / cantidad;          // ❌ → 3.0 (división entera)
float bien = (float) total / cantidad;  // ✅ → 3.333...
```

> ⚠️ `int / int` siempre da entero aunque el resultado se guarde en un `float`. Hay que castear AL MENOS uno de los dos operandos: `(float) total / cantidad`.

---

