# Unario

![operador unario](/imagenesjava/operadorunario.png "FOTO")

**Primera explicación.**

Si las utilizas en una línea donde sea la única expresión no hay ninguna diferencia, pero si las ejecutas junto con otras hay una variación importante.

* ++x lo hace antes de que se evalué la expresión. También se llama PREINCREMENTO


Ejemplo:
int x = 5;

        System.out.println(++x); // escribirá 6 porque ejecutará x + 1 ANTES de printar
        System.out.println(x);   // volverá a escribir 6!!!!

* x++ lo hace posteriormente a que la expresión sea evaluada. También se llama POSTINCREMENTO

Ejemplo:

        int x = 5;
        System.out.println(x++); // escribirá 5 porque ejecutará x + 1 DESPUÉS de printar
        System.out.println(x);   // escribirá 6


**Segunda explicación**

La diferencia no está en que el incremento se ejecute antes o después de evaluar la expresión sino en el valor de retorno de las dos expresiones

Es decir:

        int x = 5;
        System.out.println(++x);  // Imprime 6, x vale 6: El resultado de la expresión ++x es 6 y se imprime 6
        System.out.println(x); // Imprime 6, x vale 6: x ya se incrementó por lo que devuelve 6

Mientras que:


        int x = 5;
        System.out.println(x++);  // Imprime 5, x vale 6. La variable x ya es 6 pero el resultado 
                                     de la expresión es 5 por lo que se imprime 5
        System.out.println(x); // Imprime 6, x vale 6: x ya se incrementó por lo que devuelve 6
