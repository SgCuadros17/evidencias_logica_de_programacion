<!-- No borrar o modificar -->

[Inicio](./index.md)

<!-- Su documentación aquí -->

## Sesión 3

## Actividad 3: Ejercicios de operaciones básicas en Java.

1. **Suma y multiplicación:** Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

```java
import java.util.Scanner;
public class SumaMultiplicacion {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Suma y multiplicación:");
        System.out.print("Introduzca el primer número: ");
        int num1 = scanner.nextInt();
        System.out.print("Introduzca el segundo número: ");
        int num2 = scanner.nextInt();
        int suma = num1 + num2;
        int multiplicacion = num1 * num2;
        System.out.println("La suma de los dos números es: " + suma);
        System.out.println("La multiplicación de los dos números es: " + multiplicacion);
    }
}
```

2. **Resta y división:** Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

```java
import java.util.Scanner;
public class RestaDivision {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // Resta y división
        System.out.println("Resta y división:");
        System.out.print("Introduzca el primer número: ");
        int num1 = scanner.nextInt();
        System.out.print("Introduzca el segundo número: ");
        int num2 = scanner.nextInt();
        int resta = num1 - num2;
        int division = num1 / num2;
        System.out.println("La resta de los dos números es: " + resta);
        System.out.println("La división de los dos números es: " + division);
    }
}
```

3. **Operaciones combinadas:** Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

```java
import java.util.Scanner;
public class OperacionesCombinadas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // Leer los tres números del usuario
        System.out.println("Introduce el primer número:");
        int num1 = scanner.nextInt();
        System.out.println("Introduce el segundo número:");
        int num2 = scanner.nextInt();
        System.out.println("Introduce el tercer número:");
        int num3 = scanner.nextInt();
        // Realizar las operaciones
        int suma = num1 + num2 + num3;
        int multiplicacion = num1 * num2;
        int division = multiplicacion / num3;
        // Imprimir los resultados
        System.out.println("La suma de los tres números es: " + suma);
        System.out.println("La multiplicación del primer número por el segundo es: " + multiplicacion);
        System.out.println("La división del resultado entre el tercer número es: " + division);
    }
}
```

4. **Operaciones con decimales:** Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

```java
import java.util.Scanner;
public class OperacionesConDecimales {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // Leer los dos números decimales del usuario
        System.out.println("Introduce el primer número decimal:");
        double num1 = scanner.nextDouble();
        System.out.println("Introduce el segundo número decimal:");
        double num2 = scanner.nextDouble();
        // Realizar las operaciones
        double suma = num1 + num2;
        double resta = num1 - num2;
        double multiplicacion = num1 * num2;
        double division = num1 / num2;
        // Imprimir los resultados
        System.out.println("La suma de los dos números decimales es: " + suma);
        System.out.println("La resta de los dos números decimales es: " + resta);
        System.out.println("La multiplicación de los dos números decimales es: " + multiplicacion);
        System.out.println("La división de los dos números decimales es: " + division);
    }
}
```

5. **Incremento y decremento:** Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

```java
import java.util.Scanner;
public class IncrementoDecremento {
    public static void main(String[] args) {
        // Declarar una variable entera e inicializarla con un valor
        int numero = 10;
        // Incrementar su valor en 1 y mostrar el resultado
        numero++;
        System.out.println("El valor de la variable después de incrementarse es: " + numero);
        // Decrementar su valor en 1 y mostrar el resultado nuevamente
        numero--;
        System.out.println("El valor de la variable después de decrementarse es: " + numero);
    }
}
```

6. **Operador de asignación compuesta:** Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

```java
import java.util.Scanner;
public class OperadorAsignacionCompuesta {
    public static void main(String[] args) {
        int numero = 10;
        numero += 5;
        // Mostrar el valor de la variable
        System.out.println("El valor de la variable es: " + numero);
    }
}
```

7. **Operadores lógicos:** Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

```java
import java.util.Scanner;
public class OperadoresLogicos {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // Leer los dos valores booleanos del usuario
        System.out.println("Introduce el primer valor booleano:");
        boolean valor1 = scanner.nextBoolean();
        System.out.println("Introduce el segundo valor booleano:");
        boolean valor2 = scanner.nextBoolean();
        // Mostrar el resultado de las operaciones lógicas AND, OR y NOT entre esos valores
        System.out.println("El resultado de la operación lógica AND es: " + (valor1 && valor2));
        System.out.println("El resultado de la operación lógica OR es: " + (valor1 || valor2));
        System.out.println("El resultado de la operación lógica NOT del primer valor es: " + !valor1);
        System.out.println("El resultado de la operación lógica NOT del segundo valor es: " + !valor2);
    }
}
```

8. **Operador ternario:** Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado.

```java
import java.util.Scanner;
public class OperadorTernario {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Introduce un número entero:");
        int numero = scanner.nextInt();
        String resultado = (numero >= 0) ? "positivo" : "negativo";
        System.out.println("El número es " + resultado);
    }
}
```
