# 04 — Entrada y Salida

## Salida: `printf()`

```c
int edad = 25;
printf("Tengo %d años\n", edad);   // \n = salto de línea
printf("Pi es %.2f\n", 3.1416);    // → Pi es 3.14
```

## Especificadores de formato

| Especificador | Tipo |
|---|---|
| `%d` | int |
| `%f` | float |
| `%lf` | double |
| `%c` | char |
| `%s` | string (char[]) |
| `%.2f` | float con 2 decimales |
| `\n` | salto de línea |

## Entrada: `scanf()`

Se usa para leer números o palabras sueltas. El `&` es obligatorio — indica la dirección de memoria donde guardar el valor.

```c
int num;
printf("Ingresá un número: ");
scanf("%d", &num);    // & = dirección de memoria (obligatorio)

float precio;
scanf("%f", &precio);
```

## Entrada de texto con espacios: `fgets()`

`scanf("%s", ...)` se detiene en el primer espacio. Para leer frases completas usá `fgets()`.

```c
char nombre[50];
fgets(nombre, 50, stdin);  // lee hasta 50 caracteres incluyendo espacios
```

> ⚠️ Nunca uses `scanf("%s", ...)` para leer nombres o frases — no captura espacios y puede causar desbordamiento de buffer.

---

