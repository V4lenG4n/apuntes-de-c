# 🧠 MACHETE PARCIAL C (OPTIMIZADO + LOOPS)

## 🚀 ESTRUCTURA BASE
```c
#include <stdio.h>

int main() {
    return 0;
}
```

---

## 🔹 ENTRADA / SALIDA
```c
int a;
scanf("%d", &a);
printf("%d", a);
```

---

## 🔹 TIPOS DE DATOS
```c
int a = 10;
float b = 3.14;
char c = 'A';
```

---

## 🔹 CASTING
```c
float resultado = (float)5 / 2; // 2.5
```

---

## 🔹 IF / ELSE
```c
if (condicion) {

} else {

}
```

---

## 🔹 OPERADORES
Relacionales: == != > < >= <=  
Lógicos: && || !

---

# 🔁 LOOPS

## 🔹 WHILE
```c
while (condicion) {
    // codigo
}
```

## 🔹 FOR
```c
for (int i = 0; i < 10; i++) {
    // codigo
}
```

---

# 🔥 EJERCICIOS TÍPICOS UTN

## ✔ Contar del 1 al 10
```c
for (int i = 1; i <= 10; i++) {
    printf("%d\n", i);
}
```

---

## ✔ Sumar números hasta 0
```c
int num, suma = 0;

scanf("%d", &num);
while (num != 0) {
    suma += num;
    scanf("%d", &num);
}

printf("Suma: %d", suma);
```

---

## ✔ Mayor de N números
```c
int n, num, max;

scanf("%d", &n);
scanf("%d", &max);

for (int i = 1; i < n; i++) {
    scanf("%d", &num);
    if (num > max) {
        max = num;
    }
}

printf("Max: %d", max);
```

---

## ✔ Contar pares
```c
int n, num, contador = 0;

scanf("%d", &n);

for (int i = 0; i < n; i++) {
    scanf("%d", &num);
    if (num % 2 == 0) {
        contador++;
    }
}

printf("Pares: %d", contador);
```

---

# ⚠️ ERRORES COMUNES

❌ if (a = 5)  
✔️ if (a == 5)

❌ división entera  
✔️ usar casting

❌ sin llaves  
✔️ usar {}

---

# ⚡ TIPS

- Pensar casos
- Usar casting
- Revisar condiciones
