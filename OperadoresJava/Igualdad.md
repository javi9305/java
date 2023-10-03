`````` java

public static void main(String[] args) {
        
        //Declaracion de variables el cual se les asigna un valor a cada una.
        var a = 3;
        var b = 2;
        
        var c = (a==b); //se evalua la expresion si la variable a y b  son iguales y el resultado es guardado en la variable c.
        System.out.println("c = " + c); //imprime el resultado el cual es false.
        
        var d = a != b; //se evalua la expresion si la variable a y b son diferentes y el resultado es guardado en la variable d.
        System.out.println("d = " + d);//Imprime el resultado el cual es true.
        
        /*
         cuando colocamos hola en ambas cadenas el resultado de la variable 
         es true y eso se debe a que Java para la cuestión de cadenas hace
        un cache, por lo que al no usar new, se crea la cadena en la zona de
        cache de la memoria Heap, entonces es normal que si es la misma cadena 
        tome en esa zona de cache la misma referencia de la cadena, por eso 
        te da true.
        
        
        */
        
        //Creo variables de tipo cadena el cual se les asigna sus valores.
        var cadena = "hola";
        var cadena2 = "hola";
        
        var e = cadena == cadena2; //compara referencias de objetos
        System.out.println("e = " + e); //el resultado es true (ver texto de arriba).
        
        var f = cadena.equals(cadena2);//comparamos cadenas.
        System.out.println("f = " + f);
    }



`````` 