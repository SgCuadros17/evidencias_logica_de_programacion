<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 

<!-- Su documentación aquí -->

## Actividad 7: Ejecicios Array - ArrayList

1. En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.
Ejemplo Array

```java
import java.util.Arrays;
public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
```

### Ejemplo Array list

```java
import java.util.ArrayList; 
import java.util.Scanner;

public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }

  public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}
```

## Analisis. 

En el primer ejemplo, se utiliza un array de enteros para almacenar y manipular números. Se crea un array llamado "numeros" e inicializado con cinco números enteros. Luego, se calcula la suma de los elementos del array utilizando un bucle for. Además, se encuentra el número más grande en el array utilizando otro bucle for. Finalmente, se ordena el array en orden ascendente utilizando el método sort() de la clase Arrays.

En el segundo ejemplo, se utiliza un ArrayList de objetos String para almacenar y manipular notas. Se crea un ArrayList llamado "notas" e inicializado vacío. Luego, se utiliza un bucle while para ejecutar un menú que permite al usuario agregar notas, mostrar todas las notas almacenadas en el ArrayList o salir del programa. Para agregar notas, se utiliza el método add() del ArrayList. Para mostrar todas las notas, se utiliza un bucle for-each para recorrer y mostrar cada nota almacenada en el ArrayList.

2. Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.


