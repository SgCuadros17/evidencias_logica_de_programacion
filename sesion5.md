<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 

<!-- Su documentación aquí -->

## Actividad 5: Ejercicios de bucles

Resolver los siguientes ejercicios:

### Ejercicios - while

1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

```java
Scanner scanner = new Scanner(System.in);
System.out.println("Ingrese un número: ");
int numero = scanner.nextInt();
int i = 1;
while (i <= 10) {
    System.out.println(numero + " x " + i + " = " + (numero * i));
    i++;
}
```

2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

```java	
String cadena = "Hola 123";
int contador = 0;
int i = 0;
while (i < cadena.length()) {
    if (Character.isDigit(cadena.charAt(i))) {
        contador++;
    }
    i++;
}
System.out.println("Cantidad de números: " + contador);
```


## Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

```java
Scanner scanner = new Scanner(System.in);
int numero = 0;
do {
    System.out.println("Ingrese un número: ");
    numero = scanner.nextInt();
} while (numero >= 0);
```

2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

```java
Scanner scanner = new Scanner(System.in);
int numero = 0;
do {
    System.out.println("Ingrese un número: ");
    numero = scanner.nextInt();
    int i = 1;
    while (i <= 10) {
        System.out.println(numero + " x " + i + " = " + (numero * i));
        i++;
    }
} while (numero != 0);
```


## Ejercicios - for

1. Imprimir los números impares del 1 al 50.

```java
for (int i = 1; i <= 50; i++) {
    if (i % 2 != 0) {
        System.out.println(i);
    }
}
```

2. Imprimir los números primos del 1 al 100.

```java
for (int i = 1; i <= 100; i++) {
    int contador = 0;
    for (int j = 1; j <= i; j++) {
        if (i % j == 0) {
            contador++;
        }
    }
    if (contador == 2) {
        System.out.println(i);
    }
}
```






