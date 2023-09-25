<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


### Actividad 3: Ejercicios de operaciones básicas en Java.

1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

### Solución

1.
 ```java
import java.util.Scanner;

public class SumaMultiplicacion {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        int suma = numero1 + numero2;
        int multiplicacion = numero1 * numero2;

        System.out.println("La suma de los números es: " + suma);
        System.out.println("La multiplicación de los números es: " + multiplicacion);


        scanner.close();
    }
}
```
2. 

```java
import java.util.Scanner;

public class RestaDivision {
        
   public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        int resta = numero1 - numero2;
        float division = numero1 / numero2;

        System.out.println("La resta de los números es: " + resta);
        System.out.println("La division de los números es: " + division);

        
    
}
}
```
3.

```java
import java.util.Scanner;

public class OperacionesCombinadas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        System.out.print("Ingrese el tercer número entero: ");
        int numero3 = scanner.nextInt();

        int suma = numero1 + numero2 + numero3;
        float multiplicacion = numero1 * numero2;
        float division = (numero1 * numero2) / numero3;


        System.out.println("La suma de los números es: " + suma);
        System.out.println("La multiplicación de los números es: " + multiplicacion);
        System.out.println("La division de los números es: " + division);

}
}

```
4.

```java
import java.util.Scanner;

public class OperacionesconDecimales {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número: ");
         float numero1 = scanner.nextFloat();

        System.out.print("Ingrese el segundo número: ");
        float numero2 = scanner.nextFloat();

        float suma = numero1 + numero2;
        float resta = numero1 - numero2;
        float multiplicacion = numero1 * numero2;
        float division = numero1 / numero2;

        System.out.println("La suma de los números es: " + suma);
        System.out.println("La resta de los números es: " + resta);
        System.out.println("La multiplicación de los números es: " + multiplicacion);
        System.out.println("La division de los números es: " + division);

    }
}

```

5.

```java
public class IncrementoyDecremento {
    public static void main(String[] args) {
        int a = 10;

        a++;
        System.out.println(a);

       a--;
        System.out.println(a);


    }
}

```

6.

```java
import java.util.Scanner;

public class Operadorasignacioncompuesta {
    public static void main(String[] args) {

        int x = 18;

        x += 5;

        System.out.println("El valor de la variable después de sumar 5 es: " + x );

    }
}

```

7.

```java
public class Operadoreslogicos {
    public static void main(String[] args) {
        int edad = 25;

        boolean esMadre = true;
        boolean esAbuela = false;

        boolean resultado1 = (edad > 25) && esMadre;
        boolean resultado2 = esMadre || esAbuela;
        boolean resultado3 = !esMadre;

        System.out.println("El resultado 1 es: " + resultado1);
        System.out.println("El resultado 2 es: " + resultado2);
        System.out.println("El resultado 3 es: " + resultado3);
        
}
}
```

8.

```java
public class OperadorTernario {
    public static void main(String[] args) {
    
        int edad = 25;

        String mensaje = (edad <= 30) ? "Edad requerida" : "no cumple edad";
        System.out.println(mensaje);
}
}
```



