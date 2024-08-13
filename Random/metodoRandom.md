
el metodo Math.ramdom() es un metodo estatico que devuelve un numero double de 0.0 o 1.0.
       
si los numeros de 5 cifras van de 10000 a 99999, puedes generar un número aleatorio con Math.random() y escalarlo.

       Ejemplo codigo:
     
 ``````java
 double fiveDigits = 10000 + Math.random() * 90000;
 ``````
       
En caso que Math.random() devuelva el mínimo, 0, el resultado será 10000 + 0 * 90000, que es 10000.
En caso que Math.random() devuelva el máximo, 1 (exclusivo), el resultado será 10000 + 1 * 90000, que es 100000, pero como el 1 no es 1, sinó que 0.9999..., 
el resultado es realmente 10000 + 0.999... * 90000, que es 10000 + 89999.9999..., o sea 99999.999....

Una vez hagamos el casting de double a int, tendremos un número [10000, 99999].

       Ejemplo codigo
``````java       
public int getFiveDigitsNumber() {
    double fiveDigits = 10000 + Math.random() * 90000;
    return (int) fiveDigits;
}
``````