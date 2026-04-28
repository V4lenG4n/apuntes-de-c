# 🧪 EJERCICIOS TIPO EXAMEN RESUELTOS (C)

## 📌 1. Positivo / Negativo / Cero
```c
int num;
scanf("%d", &num);

if (num > 0) {
    printf("Positivo");
} else if (num < 0) {
    printf("Negativo");
} else {
    printf("Cero");
}
```

---

## 📌 2. Par o impar
```c
int num;
scanf("%d", &num);

if (num % 2 == 0) {
    printf("Par");
} else {
    printf("Impar");
}
```

---

## 📌 3. Mayor de dos números
```c
int a, b;
scanf("%d %d", &a, &b);

if (a > b) {
    printf("A es mayor");
} else if (b > a) {
    printf("B es mayor");
} else {
    printf("Son iguales");
}
```

---

## 📌 4. Rango de edad
```c
int edad;
scanf("%d", &edad);

if (edad < 18) {
    printf("Menor");
} else if (edad < 65) {
    printf("Adulto");
} else {
    printf("Jubilado");
}
```

---

## 📌 5. Nota
```c
int nota;
scanf("%d", &nota);

if (nota >= 6) {
    printf("Aprobado");
} else {
    printf("Desaprobado");
}
```

---

## 📌 6. Suma hasta 0
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

## 📌 7. Contar pares
```c
int n, num, cont = 0;

scanf("%d", &n);

for (int i = 0; i < n; i++) {
    scanf("%d", &num);
    if (num % 2 == 0) {
        cont++;
    }
}

printf("Pares: %d", cont);
```

---

## 📌 8. Mayor de N números
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

## 📌 9. Tabla de multiplicar
```c
int num;
scanf("%d", &num);

for (int i = 1; i <= 10; i++) {
    printf("%d x %d = %d\n", num, i, num * i);
}
```

---

## 📌 10. Validación
```c
int num;

scanf("%d", &num);

while (num < 1 || num > 10) {
    printf("Error, ingrese de nuevo: ");
    scanf("%d", &num);
}

printf("Valido");
```

---

# ⚡ PATRONES CLAVE

- Contador → variable que suma dentro de un loop
- Acumulador → suma valores
- Máximo → comparar y guardar
- Validación → while con condición incorrecta
