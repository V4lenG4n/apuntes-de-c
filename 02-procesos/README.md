# 02 — Procesos y Estados

Un **proceso** es un programa en ejecución. El sistema operativo le asigna memoria, CPU y recursos. Cada proceso tiene un **PID** único.

## Regiones de memoria de un proceso

| Región | Qué contiene |
|---|---|
| Código (texto) | Las instrucciones del programa |
| Datos | Variables globales y estáticas |
| Heap | Memoria dinámica (`malloc`, `calloc`, `free`) |
| Stack | Variables locales y llamadas a funciones |

## Obtener el PID

```c
#include <stdio.h>
#include <unistd.h>

int main() {
    // getpid() devuelve el identificador del proceso actual
    printf("Mi PID es: %d\n", getpid());
    return 0;
}
```

---


