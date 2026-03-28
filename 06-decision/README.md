# 06 — Estructuras de Decisión

## `if` simple

Ejecuta el bloque solo si la condición es verdadera.

```c
if (edad >= 18) {
    printf("Mayor de edad\n");
}
```

## `if-else`

Dos caminos: uno si es verdadero, otro si es falso.

```c
if (numero % 2 == 0) {
    printf("Par\n");
} else {
    printf("Impar\n");
}
```

## `if` anidado

Un `if` dentro de otro para evaluar varias condiciones en cadena.

```c
if (numero >= 0) {
    if (numero == 0) {
        printf("Cero\n");
    } else {
        printf("Positivo\n");
    }
} else {
    printf("Negativo\n");
}
```

## `switch`

Compara una variable contra valores fijos. Más limpio que muchos `if-else` seguidos.

```c
switch(dia) {
    case 1:
        printf("Lunes\n");
        break;     // sin break, continúa al siguiente case
    case 2:
        printf("Martes\n");
        break;
    case 6:
    case 7:        // dos casos con el mismo resultado
        printf("Fin de semana\n");
        break;
    default:       // si ningún case coincide
        printf("Otro\n");
}
```

## Cuándo usar cada uno

| Estructura | Cuándo usarla |
|---|---|
| `if` | Una condición simple |
| `if-else` | Dos resultados posibles |
| `if` anidado | Varias decisiones dependientes |
| `switch` | Comparar un valor contra muchas opciones fijas |

## Errores comunes

> ⚠️ **Error 1:** usar `=` en lugar de `==` en condiciones.  
> `if (x = 5)` asigna el valor 5 a x, no compara. Siempre usá `==`.

> ⚠️ **Error 2:** olvidar el `break` en switch.  
> Sin `break`, el código "cae" al siguiente case y lo ejecuta también.

---

