<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 

<!-- Su documentación aquí -->
## Actividad 10: Prueba, ejecución y explicación de ejercicios de lógica de programación.

Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno.

### Ejercicio 1: Cantidad de ladrillos:

```java
import java.util.Scanner;

public class CantidadLadrillos {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo;
      
      // Solicita las dimensiones de la pared
      System.out.print("Ingrese el largo de la pared en metros: ");
      largo = input.nextDouble();
      System.out.print("Ingrese el alto de la pared en metros: ");
      alto = input.nextDouble();
      System.out.print("Ingrese el ancho de la pared en metros: ");
      ancho = input.nextDouble();

      // Solicita las dimensiones del ladrillo
      System.out.print("Ingrese el largo del ladrillo en metros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en metros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en metros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}
```
Calcula la cantidad de ladrillos necesarios para construir una pared. El programa solicita al usuario las dimensiones de la pared (largo, alto y ancho) y las dimensiones del ladrillo (largo, alto y ancho). A continuación, calcula el área de la pared y el área del ladrillo. Por último, calcula la cantidad de ladrillos necesarios dividiendo el área de la pared por el área del ladrillo.
El programa utiliza la clase `Scanner` para obtener la entrada del usuario. La clase `Scanner` proporciona métodos para leer diferentes tipos de datos, como números y cadenas. El programa utiliza el método `nextDouble()` para leer los números introducidos por el usuario.
El programa utiliza la clase `Math` para realizar cálculos matemáticos. La clase `Math` proporciona métodos para realizar operaciones matemáticas comunes, como la suma, la resta, la multiplicación y la división. El programa utiliza el método `ceil()` para redondear un número al entero más cercano.
El programa utiliza la clase `System` para mostrar la salida en la consola. La clase `System` proporciona métodos para mostrar mensajes en la consola. El programa utiliza el método `printf()` para mostrar un mensaje formateado en la consola.


### Ejercicio 2: Calcular el índice de masa corporal (IMC) de una persona:

```java
import java.util.Scanner;

public class IMC {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double weight, height, imc;
      
      // Solicita el peso y la altura
      System.out.print("Ingrese su peso en kilogramos: ");
      weight = input.nextDouble();
      System.out.print("Ingrese su altura en metros: ");
      height = input.nextDouble();

      // Calcula el IMC
      imc = weight / (height * height);

      // Muestra el resultado en la consola
      System.out.printf("Su IMC es %.2f", imc);
   }
}
```
El IMC es una medida de la grasa corporal basada en la altura y el peso de una persona. Se calcula dividiendo el peso de una persona en kilogramos por el cuadrado de su altura en metros.
El programa primero importa la clase Scanner de la biblioteca java.util. La clase Scanner se utiliza para obtener la entrada del usuario. El programa luego define una clase llamada IMC con un método principal. El método principal es el punto de entrada del programa.
El método principal primero crea un objeto Scanner para obtener la entrada del usuario. Luego, solicita al usuario que ingrese su peso en kilogramos y su altura en metros. El programa luego usa la clase Math para calcular el IMC de la persona. Finalmente, el programa muestra el IMC de la persona en la consola.



