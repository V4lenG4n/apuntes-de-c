# 07 — Sentencias de Iteración

## `while`

Repite el bloque **mientras** la condición sea verdadera. La condición se evalúa **antes** de ejecutar.

```c
int i = 1;
while (i <= 5) {
    printf("%d\n", i);
    i++;           // actualizar siempre o bucle infinito
}
// Salida: 1 2 3 4 5
```

## `do-while`

Igual que `while`, pero la condición se evalúa **al final**. Se ejecuta **al menos una vez** aunque la condición sea falsa desde el principio.

```c
int j = 1;
do {
    printf("%d\n", j);
    j++;
} while (j <= 5);  // condición AL FINAL
// Salida: 1 2 3 4 5
```

```c
// Ejemplo donde se ejecuta aunque la condición sea falsa
int numero = 10;
do {
    printf("Se ejecutó una vez igual\n");
} while (numero < 5);   // falso, pero ya se ejecutó
```

## `for`

Ideal cuando sabés exactamente cuántas veces repetir. Tiene tres partes en una línea.

```c
//    inicio     condición  actualización
for (int k = 1; k <= 5;    k++) {
    printf("%d\n", k);
}
// 1. int k=1  → se ejecuta UNA sola vez al inicio
// 2. k<=5     → se verifica ANTES de cada iteración
// 3. k++      → se ejecuta AL FINAL de cada iteración
```

## Comparación

| Bucle | Cuándo usarlo | Evalúa la condición |
|---|---|---|
| `while` | No sé cuántas veces | Antes — puede no ejecutarse nunca |
| `do-while` | Necesito ejecutar al menos una vez | Después — mínimo 1 ejecución |
| `for` | Sé exactamente cuántas veces | Antes de cada iteración |

## Errores comunes

> ⚠️ **Bucle infinito:** si la variable del ciclo nunca cambia, el programa se cuelga.

```c
// ❌ Bucle infinito — i nunca cambia
int i = 1;
while (i <= 5) {
    printf("%d\n", i);
    // falta i++
}

// ✅ Correcto
while (i <= 5) {
    printf("%d\n", i);
    i++;
}
```

---


