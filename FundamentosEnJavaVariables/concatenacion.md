`````` java

//Este programa realiza la concatenacion primero de 2 String y luego de enteros y un String.

package VariablesEnJava;

public class Concatenacion {
    //la concatenacion es unir varios valores el cual deben ser tipo string o char
   //Metodo principal main
    public static void main(String[] args) {
        
        //Declaracion de variables tipo String la cual se les asigna valores por default.
        var usuario = "Juan";
        var titulo = "Ingeniero";

        //concatenando las dos variables  y asignandola a una nueva variable la cual sera impresa en consola.
        var union = titulo + " " + usuario;
        System.out.println("union = " + union);
        
        //Declaracion de variables tipo entero la cual se les asigna valores por default.
        var i = 3;
        var j = 4;
        
        System.out.println(i + j);//se realiza la suma de numeros.

        /*
        //Evaluacion de izq a der y posteriormente realiza suma 
        y luego se concatena el valor de la cadena.
        */
        System.out.println(i + j + usuario);
        
        System.out.println(usuario + i + j);//Contexto cadena,todo es una cadena es decir todo lo toma como una cadena.
        System.out.println(usuario + (i + j));//Uso de parentesis modifican la prioridad en la evaluacion.
        
        
        
    }
    
}

`````` 