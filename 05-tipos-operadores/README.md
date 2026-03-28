# 05 — Tipos de Datos y Operadores

## Operadores

| Grupo | Operadores | Ejemplo | Resultado |
|---|---|---|---|
| Aritméticos | `+ - * / %` | `10 % 3` | `1` (resto) |
| Relacionales | `== != > < >= <=` | `edad >= 18` | `1` (true) o `0` (false) |
| Lógicos | `&& \|\| !` | `a > 0 && b > 0` | true si ambos son positivos |
| Asignación | `= += -= *= /=` | `x += 5` | equivale a `x = x + 5` |
| Incremento | `++ --` | `i++` | equivale a `i = i + 1` |

## Precedencia (orden de evaluación)

De mayor a menor prioridad:

```
( )           → paréntesis, primero siempre
* / %         → multiplicación, división, módulo
+ -           → suma y resta
> < >= <=     → relacionales
== !=         → igualdad
&&            → AND lógico
||            → OR lógico
```

```c
// Ejemplo
int r = 2 + 3 * 4;      // → 14  (primero 3*4=12, luego 2+12)
int s = (2 + 3) * 4;    // → 20  (paréntesis primero)
```

## Operador módulo `%`

Devuelve el **resto** de una división entera. Muy usado para saber si un número es par o impar.

```c
10 % 3  // → 1  (10 = 3*3 + 1)
8  % 2  // → 0  (par)
7  % 2  // → 1  (impar)

if (numero % 2 == 0) {
    printf("Es par\n");
}
```

---


