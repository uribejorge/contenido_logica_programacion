<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->


# Estructuras de control en Java
Las estructuras de control en Java son construcciones del lenguaje que permiten controlar el flujo de ejecución de un programa. Los principales tipos de estructuras de control en Java son:

- Estructuras de selección: permiten elegir entre varias opciones. Incluyen la sentencia if, la sentencia switch.

- Estructuras repetitivas: permiten repetir un bloque de código mientras se cumpla una condición. Incluyen los bucles for, while, do-- while.

- Estructuras de salto: permiten cambiar el flujo de ejecución, saltando parte del código. Incluyen las sentencias break, continue, return.

## Estructuras condicionales:
Las estructuras condicionales en Java permiten tomar decisiones y ejecutar ciertas partes de código dependiendo si se cumple o no una determinada condición.

Las principales estructuras condicionales son:

1. ## if: Ejecuta un bloque de código si se cumple la condición.
Sintaxis:

```

if (condición) {
  // código a ejecutar 
}

```

2. ## if - else: Ejecuta un bloque si se cumple la condición, y otro bloque distinto si no se cumple.
Sintaxis:

```

if (condición) {
  // código si se cumple
} else {
  // código si no se cumple
}

```

3. ## if - else if - else: Permite evaluar múltiples condiciones. Se ejecuta el primer bloque donde se cumpla la condición.
Sintaxis:

```

if (condición 1) {
  // código si se cumple 1
} else if (condición 2) {
  // código si se cumple 2 
} else {
  // código si no se cumple ninguna
}

```

4. ## Operador ternario
El operador ternario en Java es una expresión que se utiliza para evaluar una condición y devolver uno de dos valores, dependiendo del resultado de la evaluación. La sintaxis del operador ternario es:

Sintaxis:

``variable = (condicion) ? valor_si_verdadero : valor_si_falso;``

5. ## switch: Evalúa una variable o expresión y ejecuta el código del case que coincida con el valor.
Sintaxis:

```

switch(expresión) {
  case valor1: 
    //código
    break;
  case valor2: 
   //código
   break;
  default:
   //código por defecto  
}

```

Estas estructuras permiten controlar el flujo del programa ejecutando código de manera condicional. Son muy útiles para realizar selecciones y tomar decisiones en la lógica de un programa.

## Ejemplos if:
Estos ejemplos muestran diferentes formas de utilizar estructuras condicionales en Java para tomar decisiones basadas en ciertas condiciones.


1. ## Comprobando si una variable es mayor que otra:

```

int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
}

```

2. ## Comprobando si una variable es diferente de un valor específico:

```

int edad = 18;

if (edad != 18) {
  System.out.println("La edad no es 18");
}

```

3. ## Comprobando si una variable está dentro de un rango de valores:

```

int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
}

```

## Ejemplos if else:
1. ## Comprobando si una variable es mayor que otra y, si no, imprimiendo un mensaje diferente:

```

int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
} else {
  System.out.println("x es menor o igual que y");
}

```

2. ## Comprobando si una variable es igual a un valor específico y, si no, imprimiendo un mensaje diferente:

```

String nombre = "Juan";

if (nombre.equals("Juan")) {
  System.out.println("El nombre es Juan");
} else {
  System.out.println("El nombre no es Juan");
}

3. Comprobando si una variable está dentro de un rango de valores y, si no, imprimiendo un mensaje diferente:
int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
} else {
  System.out.println("La nota no es excelente");
}

Ejemplos else if:
1. Comprobando si una variable es mayor que otra, si no, si es igual y, si no, imprimiendo un mensaje diferente:
int x = 10;
int y = 5;

if (x > y) {
  System.out.println("x es mayor que y");
} else if (x == y) {
  System.out.println("x es igual a y");
} else {
  System.out.println("x es menor que y");
}

```

2. ## Comprobando si una variable está dentro de un rango de valores, si no, si es mayor o si es menor y, si no, imprimiendo un mensaje diferente:

```

int nota = 10;

if (nota >= 9 && nota <= 10) {
  System.out.println("La nota es excelente");
} else if (nota > 10) {
  System.out.println("La nota es sobresaliente");
} else if (nota < 0) {
  System.out.println("La nota es inválida");
} else {
  System.out.println("La nota es buena");
}

```

3. ## Comprobando si una variable está vacía o no, si no, si tiene una longitud específica y, si no, imprimiendo un mensaje diferente:

```

String cadena = "";

if (cadena.isEmpty()) {
  System.out.println("La cadena está vacía");
} else if (cadena.length() == 0) {
  System.out.println("La cadena es nula");
} else {
  System.out.println("La cadena no está vacía");
}

```

### Ejemplos operador ternario:
1. ### Devuelve el valor máximo de dos números

```

int max = (a > b) ? a : b;

// Devuelve el texto "El número es positivo" si el número es mayor que 0,
// y el texto "El número es negativo" si el número es menor o igual a 0.
String texto = (numero > 0) ? "El número es positivo" : "El número es negativo";

```

2. ### Devuelve el valor máximo de tres números

```

int max = (a > b) ? (a > c ? a : c) : (b > c ? b : c);

// Devuelve el texto "El número es positivo" si el número es mayor que 0,
// el texto "El número es cero" si el número es igual a 0,
// y el texto "El número es negativo" si el número es menor que 0.
String texto = (numero > 0) ? "El número es positivo" : (numero == 0 ? "El número es cero" : "El número es negativo");

```

3. ### Devuelve el texto "El número es par" si el número es par, y el texto "El número es impar" si el número es impar.

```

String texto = (numero % 2 == 0) ? "El número es par" : "El número es impar";

```

### Otros ejemplos
1. ### Comprobación del número par o impar:

```

int numero = 7;

if (numero % 2 == 0) {
    System.out.println("El número es par.");
} else {
    System.out.println("El número es impar.");
}

```

2. ### Evaluación de la calificación de un estudiante:

```

int calificacion = 85;

if (calificacion >= 90) {
    System.out.println("Excelente");
} else if (calificacion >= 80) {
    System.out.println("Bueno");
} else if (calificacion >= 70) {
    System.out.println("Regular");
} else {
    System.out.println("Reprobado");
}

```

3. ### Verificación de la elegibilidad para votar:

```

int edad = 17;

if (edad >= 18) {
    System.out.println("Eres elegible para votar.");
} else {
    System.out.println("No eres elegible para votar.");
}

```

4. ### Determinar si un número es positivo, negativo o cero:

```

int numero = -3;

if (numero > 0) {
    System.out.println("El número es positivo.");
} else if (numero < 0) {
    System.out.println("El número es negativo.");
} else {
    System.out.println("El número es cero.");
}

```

5. ### Validación de una contraseña:

```

String contraseña = "secreta123";

if (contraseña.equals("secreta123")) {
    System.out.println("Contraseña correcta. Acceso concedido.");
} else {
    System.out.println("Contraseña incorrecta. Acceso denegado.");
}

```

### Ejemplos switch:
1. ### Escribe un programa que le pida al usuario que ingrese un día de la semana. El programa debe imprimir el número del día de la semana.

```

import java.util.Scanner;

public class DiaSemana {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese un día de la semana: ");
    String dia = sc.nextLine();

    switch (dia) {
      case "lunes":
        System.out.println("1");
        break;
      case "martes":
        System.out.println("2");
        break;
      case "miércoles":
        System.out.println("3");
        break;
      case "jueves":
        System.out.println("4");
        break;
      case "viernes":
        System.out.println("5");
        break;
      case "sábado":
        System.out.println("6");
        break;
      case "domingo":
        System.out.println("7");
        break;
      default:
        System.out.println("Día no válido");
    }
  }
}

```

2. ### Escribe un programa que le pida al usuario que ingrese una calificación de 1 a 10. El programa debe imprimir la calificación en letras.

```

import java.util.Scanner;

public class Calificacion {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese una calificación de 1 a 10: ");
    int calificacion = sc.nextInt();

    switch (calificacion) {
      case 1:
        System.out.println("Insuficiente");
        break;
      case 2:
        System.out.println("Insuficiente");
        break;
      case 3:
        System.out.println("Insuficiente");
        break;
      case 4:
        System.out.println("Suficiente");
        break;
      case 5:
        System.out.println("Bien");
        break;
      case 6:
        System.out.println("Notable");
        break;
      case 7:
        System.out.println("Sobresaliente");
        break;
      case 8:
        System.out.println("Sobresaliente");
        break;
      case 9:
        System.out.println("Sobresaliente");
        break;
      case 10:
        System.out.println("Excelente");
        break;
      default:
        System.out.println("Calificación no válida");
    }
  }
}

```

3. ### Escribe un programa que le pida al usuario que ingrese un número entero. El programa debe imprimir la estación del año correspondiente al número.

```

import java.util.Scanner;

public class Estacion {

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Ingrese un número entero: ");
    int numero = sc.nextInt();

    switch (numero) {
      case 1:
      case 2:
      case 3:
        System.out.println("Invierno");
        break;
      case 4:
      case 5:
      case 6:
        System.out.println("Primavera");
        break;
      case 7:
      case 8:
      case 9:
        System.out.println("Verano");
        break;
      case 10:
      case 11:
      case 12:
        System.out.println("Otoño");
        break;
      default:
        System.out.println("Número no válido");
    }
  }
}


```


