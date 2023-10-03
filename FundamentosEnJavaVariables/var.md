# Inferencia de tipos java - var
**Se usa el var a partir de la versión 10 del jdk, ademas es opcional**

`````` java
        //Al utilizar var tiene una restriccion es decir que puede usarse en una sola linea. -> si lo hacemos asi: var a = 3, b = 4; -> marcaria error. 
        var miVariableEntera2 = 15; //Asigno un valor entero a la variable la cual sabra que es un numero entero(Inferencia de tipos)
        System.out.println(miVariableEntera2); //Imprime el valor de la variable

        var miVariableCadena2 = "Nueva Cadena"; //Asigno una cadena a una variable la cual sabra que es una cadena.
        System.out.println("miVariableCadena2 = " + miVariableCadena2);//Concadena un texto junto con la variable.



       var numeroEntero = 10;
       var numeroDouble = 10.0;
       var numeroFloat = 10.0F;

/*
     Para ver paso a paso la ejecucion del programa.

       se coloca el punto de ruptura sobre el numero de la linea de codigo,
       click derecho ->Debug File ->Step Over(F8).
    
       En caso de que no se visualice el tipo de variables ir a Window->Debugging
       
     */




``````