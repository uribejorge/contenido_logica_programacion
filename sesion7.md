<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Su documentación aquí -->


Métodos en Java
En Java, una función se llama método y es una sección de código que realiza una tarea específica y puede ser invocada (llamada) desde otras partes del programa. Los métodos pueden tener parámetros de entrada y pueden devolver un valor como resultado.

Aquí hay un ejemplo básico de cómo se puede definir una función en Java:

public int suma(int a, int b) {
    int resultado = a + b;
    return resultado;
}

Este método se llama suma, toma dos argumentos de tipo int llamados a y b, y devuelve un resultado de tipo int. El código dentro del método simplemente suma los dos argumentos y devuelve el resultado.

Para llamar a este método desde otra parte del programa, se puede hacer lo siguiente:

int x = 5;
int y = 7;
int z = suma(x, y);
System.out.println(z);

En este ejemplo, se llama al método suma pasando los valores x e y como argumentos. El resultado se almacena en la variable z y se imprime en la consola.

Funciones que no recibe parámetros y no retorna nada
En Java, las funciones que no reciben parámetros y no retornan nada se conocen como "métodos" y se declaran utilizando la palabra clave "void". Aquí hay un ejemplo de una función en Java que no recibe parámetros y no retorna nada:

public void saludar() {
    System.out.println("Hola, bienvenido/a!");
}

En este ejemplo, la función se llama "saludar" y no recibe ningún parámetro. La palabra clave "public" indica que la función es visible desde cualquier parte del programa. La palabra clave "void" indica que la función no retorna nada.

Dentro de la función, se utiliza el método "println" de la clase "System" para imprimir el mensaje "Hola, bienvenido/a!" en la consola. Esta función puede ser llamada desde cualquier parte del programa de la siguiente manera:

saludar();

Esto llamará a la función "saludar" y ejecutará su código, imprimiendo el mensaje en la consola.

Funciones que no recibe parámetros y retorna un valor
En Java, una función que no recibe parámetros y retorna un valor se conoce como una función sin argumentos. A continuación se muestra un ejemplo de una función sin argumentos que devuelve un valor:

public int obtenerNumeroAleatorio() {
   // Generar un número aleatorio entre 1 y 10
   int numeroAleatorio = (int)(Math.random() * 10) + 1;
   // Devolver el número aleatorio generado
   return numeroAleatorio;
}

En este ejemplo, la función obtenerNumeroAleatorio no recibe ningún argumento, pero genera un número aleatorio entre 1 y 10 y lo devuelve como un valor entero.

Para llamar a esta función desde otro lugar del programa, simplemente se puede hacer lo siguiente:

int numero = obtenerNumeroAleatorio();
System.out.println("El número aleatorio generado es: " + numero);

Esto imprimirá el número aleatorio generado por la función en la consola.

Funciones que reciben parámetros y retorna un valor
En Java, una función que recibe parámetros y retorna un valor se define especificando el tipo de dato que retorna la función en lugar de void. Un ejemplo de una función así podría ser:

public int sumar(int numero1, int numero2) {
    int resultado = numero1 + numero2;
    return resultado;
}

En este ejemplo, la función sumar recibe dos parámetros de tipo int y devuelve un valor de tipo int. La función suma los dos números que recibe como parámetros y devuelve el resultado.

Esta función se puede llamar desde otra parte del programa de la siguiente manera:

int resultado = sumar(5, 7);

En este ejemplo, el método sumar devuelve un valor de tipo entero, que es la suma de los dos parámetros a y b.

Diferencia entre función y método
En Java, el término "función" y "método" se utilizan indistintamente para referirse a bloques de código que realizan una tarea específica. Sin embargo, hay una sutil diferencia entre ambos términos.

Una función es un bloque de código que se define fuera de cualquier clase y se utiliza para realizar una tarea específica. Por lo general, se utiliza el término "función" en el contexto de la programación estructurada.

Por otro lado, un método es un bloque de código que se define dentro de una clase y se utiliza para realizar una tarea específica en el objeto de la clase. Por lo general, se utiliza el término "método" en el contexto de la programación orientada a objetos.

En resumen, la principal diferencia entre una función y un método en Java es que una función es un bloque de código independiente que se puede utilizar en cualquier parte del programa, mientras que un método es un bloque de código que está asociado con un objeto específico de una clase y se utiliza para realizar una tarea en ese objeto.

Otra diferencia importante es que los métodos tienen acceso a los campos y atributos de los objetos de la clase, mientras que las funciones no tienen acceso a los campos y atributos de los objetos.

Ejercicios resueltos
Crear un método en Java que reciba como parámetro un número entero y devuelva una cadena indicando si el número es par o impar. Si el número es par, la cadena debe ser "El número es par", y si es impar, la cadena debe ser "El número es impar".
public String parImpar(int numero) {
    if (numero % 2 == 0) {
        return "El número es par";
    } else {
        return "El número es impar";
    }
}

En este ejemplo, el método parImpar recibe un parámetro de tipo int y utiliza una estructura condicional if-else para determinar si el número es par o impar. Si el número es divisible por 2, entonces es par y se devuelve la cadena "El número es par". De lo contrario, se devuelve la cadena "El número es impar".

Crear un método en Java que reciba como parámetro una cadena de texto y devuelva una cadena indicando si la longitud de la cadena es mayor, menor o igual a 10 caracteres. Si la longitud de la cadena es mayor a 10, la cadena devuelta debe ser "La cadena es larga". Si la longitud de la cadena es menor a 10, la cadena devuelta debe ser "La cadena es corta". Si la longitud de la cadena es igual a 10, la cadena devuelta debe ser "La cadena tiene una longitud adecuada".
public String longitudCadena(String cadena) {
    if (cadena.length() > 10) {
        return "La cadena es larga";
    } else if (cadena.length() < 10) {
        return "La cadena es corta";
    } else {
        return "La cadena tiene una longitud adecuada";
    }
}

En este ejemplo, el método longitudCadena recibe un parámetro de tipo String y utiliza una estructura condicional if-else para determinar si la longitud de la cadena es mayor, menor o igual a 10 caracteres. Si la longitud de la cadena es mayor a 10, se devuelve la cadena "La cadena es larga". Si la longitud de la cadena es menor a 10, se devuelve la cadena "La cadena es corta". Si la longitud de la cadena es igual a 10, se devuelve la cadena "La cadena tiene una longitud adecuada".

Crear un método en Java que reciba como parámetro un número entero del 1 al 7 y devuelva una cadena indicando el nombre del día de la semana correspondiente. Para esto, se utilizará una estructura switch. Si el número es 1, se debe devolver la cadena "Lunes". Si el número es 2, se debe devolver la cadena "Martes". Si el número es 3, se debe devolver la cadena "Miércoles". Si el número es 4, se debe devolver la cadena "Jueves". Si el número es 5, se debe devolver la cadena "Viernes". Si el número es 6, se debe devolver la cadena "Sábado". Si el número es 7, se debe devolver la cadena "Domingo". Si el número está fuera del rango del 1 al 7, se debe devolver la cadena "Número inválido".
public String diaSemana(int numero) {
    switch (numero) {
        case 1:
            return "Lunes";
        case 2:
            return "Martes";
        case 3:
            return "Miércoles";
        case 4:
            return "Jueves";
        case 5:
            return "Viernes";
        case 6:
            return "Sábado";
        case 7:
            return "Domingo";
        default:
            return "Número inválido";
    }
}

En este ejemplo, el método diaSemana recibe un parámetro de tipo int que representa un número del 1 al 7. Se utiliza una estructura switch para determinar el nombre del día de la semana correspondiente. Si el número es 1, se devuelve la cadena "Lunes". Si el número es 2, se devuelve la cadena "Martes". Si el número es 3, se devuelve la cadena "Miércoles". Si el número es 4, se devuelve la cadena "Jueves". Si el número es 5, se devuelve la cadena "Viernes". Si el número es 6, se devuelve la cadena "Sábado". Si el número es 7, se devuelve la cadena "Domingo". Si el número está fuera del rango del 1 al 7, se devuelve la cadena "Número inválido".

Crear un método en Java que reciba como parámetro un número entero positivo y devuelva la suma de los números naturales desde 1 hasta el número ingresado. Para esto, se utilizará un ciclo for. Si se ingresa un número negativo o cero, se debe devolver 0.
public int sumaNaturales(int numero) {
    int suma = 0;
    if (numero <= 0) {
        return 0;
    } else {
        for (int i = 1; i <= numero; i++) {
            suma += i;
        }
        return suma;
    }
}

En este ejemplo, el método sumaNaturales recibe un parámetro de tipo int. Si el número es negativo o cero, se devuelve 0. De lo contrario, se utiliza un ciclo for para sumar los números naturales desde 1 hasta el número ingresado. La variable suma se inicializa en 0 y en cada iteración del ciclo for, se le suma el valor de i. Finalmente, se devuelve la variable suma que contiene la suma de los números naturales.

Crear un método en Java que reciba como parámetro un arreglo de números enteros y devuelva la suma de todos los elementos del arreglo. Para esto, se utilizará un ciclo for. Si se ingresa un arreglo vacío o nulo, se debe devolver 0.
public int sumarArreglo(int[] arreglo) {
    if (arreglo == null || arreglo.length == 0) {
        return 0;
    } else {
        int suma = 0;
        for (int i = 0; i < arreglo.length; i++) {
            suma += arreglo[i];
        }
        return suma;
    }
}

En este ejemplo, el método sumarArreglo recibe un parámetro de tipo int[] que representa un arreglo de números enteros. Si el arreglo es nulo o vacío, se devuelve 0. De lo contrario, se utiliza un ciclo for para recorrer cada elemento del arreglo y sumarlos. La variable suma se inicializa en 0 y en cada iteración del ciclo for, se le suma el valor del elemento del arreglo. Finalmente, se devuelve la variable suma que contiene la suma total de los elementos del arreglo.
