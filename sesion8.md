<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 

<!-- Su documentación aquí -->

## Actividad 8: Ejecicios de métodos en Java

Implementar los siguientes métodos:

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

```java
public static int max(int a, int b) {
    if (a > b) {
        return a;
    } else {
        return b;
    }
}
```

2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

```java
public static int countVowels(String text) {
    int count = 0;
    for (int i = 0; i < text.length(); i++) {
        char c = text.charAt(i);
        if (c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u') {
            count++;
        }
    }
    return count;
}
```

3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

```java
public static String swapCase(String text) {
    String result = "";
    for (int i = 0; i < text.length(); i++) {
        char c = text.charAt(i);
        if (Character.isUpperCase(c)) {
            result += Character.toLowerCase(c);
        } else {
            result += Character.toUpperCase(c);
        }
    }
    return result;
}
```

4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

```java
public static int countWords(String text) {
    int count = 0;
    for (int i = 0; i < text.length(); i++) {
        char c = text.charAt(i);
        if (c == ' ') {
            count++;
        }
    }
    return count + 1;
}
```

5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

```java
public static String sortWords(String text) {
    String[] words = text.split(" ");
    Arrays.sort(words);
    return String.join(" ", words);
}
```







