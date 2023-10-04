

`````` java

public static void main(String[] args) {

      /*
       el operador ternario es un operador condicional  y nos puede ayudar para simplificar  una estructura de tipo if/else

       var resultado (expresion que se evalua) ? true -> corresponde a la seccion en caso de que la expresion sea verdadera : false -> y despues de los 2 puntos tiene la 
       seccion que corresponde si la expresion es falsa, entonces se ejecuta esta parte del codigo.

       
      el operador ternario se recomienda utilizar si son expresiones sencillas y si son expresiones mas complejas se recomienda usar if/else.
      



      */


        
        //Verifico si el numero 3 es mayor que 2 usando el operador ?.
        var resultado = (3 > 2) ? "verdadero " : false ; //puede regresar un string o un boolean y se asigna a la variable resultado.
        System.out.println("resultado = " + resultado);
        
        //Verifico si el numero asignado por default es un numero par o impar
      var numero = 8;
      resultado = (numero % 2 == 0) ? "Numero par" : "Numero impar"; //si el resultado de la expresion es numero par se asigna a la variable resultado.
        System.out.println("resultado = " + resultado);  
    }

    ``````