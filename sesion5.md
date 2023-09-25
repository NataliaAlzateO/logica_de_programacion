<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


## Actividad 5: Ejercicios de bucles

Resolver los siguientes ejercicios:

### Ejercicios - while

1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

## Solución

1

```java
import java.util.Scanner;

public class While1 {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingrese un número: ");
        int numero = scanner.nextInt();

        int i = 1;
        while (i <= 10) {
            int resultado = numero * i;
            System.out.println(numero + " x " + i + " = " + resultado);
            i++;
        }

        scanner.close();
    }
}
```

2


```java
import java.util.Scanner;

public class While2 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = sc.nextLine();

        int i = 0;
        int contadorNumeros = 0;

        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4' || caracter == '5' || caracter == '6' || caracter == '7' || caracter == '8' || caracter == '9' || caracter == '0') contadorNumeros++;{
        }
            i++;
    }

    System.out.println("La cadena ingresada contiene "+ contadorNumeros +" Numeros.");

        }
    }
```

### Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

## Solución

1

```java
import java.util.Scanner;

public class DoWhile1 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
       
        int numero;
        

        do {
            System.out.println("Introduce un numero (o un numero negativo para detenerse): ");
            numero = scanner.nextInt();

        

        if (numero >= 0) {
            for (int i = 1; i <= 100; i++){
            System.out.println(i);
            }
        } else {
            System.out.println("Programa detenido");
        } 
        
    }while (numero >= 0);

    
        scanner.close();
    
}
}
```

2

```java
import java.util.Scanner;

public class DoWhile2 {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int b;

        do {
            System.out.println("Ingrese un numero (o ungresa 0 para salir): ");
            b = scanner.nextInt();

            if (b != 0) {
                System.out.println("Tabla de multiplicar de" + b + ":");

                for (int i = 1; i <= 10; i++) {
                    System.out.println(b + "*" + i + "=" + (b * i));
                }
            } else {
                System.out.println("Programa detenido. ");
            }
        } while (b != 0);

        scanner.close();

    }
}
```

## Ejercicios - for

1. Imprimir los números impares del 1 al 50.

2. Imprimir los números primos del 1 al 100.


## Solución

1

```java
public class For1 {
    public static void main(String[] args) {
        for (int i = 1; i <= 50; i += 2) {
            System.out.println(i);
        }
    }
}
    

```

2

```java
import java.util.Scanner;

public class For2 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        boolean primo;
        System.out.println("Son numeros primos del 1 al 100: \n");

        for (int x = 2; x <= 100; x++) {
            primo = true;
            for (int i = x - 1; i > 1; i--) {
                if (x % i == 0) {
                    primo = false;
                    break;
                }
            }
            if (primo) {
                System.out.println(x + "es primo");
            }

        }
    }

}

```




