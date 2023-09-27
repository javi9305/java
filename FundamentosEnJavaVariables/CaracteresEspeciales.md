
`````` java

//los caracteres especiales sirven para dar formato cuando se imprime en consola.
public class CaracteresEspeciales {

   //Metodo principal main.
    public static void main(String[] args) {
        
        var nombre = "Karla"; //se declara una variable la cual se le asigna un valor por default.
        
        //Impresion de los diferentes caracteres especiales.
        System.out.println("Nueva linea: \n" + nombre);
        System.out.println("Tabulador: \t" + nombre);//CARACTER TABULADOR
        System.out.println("Retroceso: \b\b" +nombre); //REGRESA UNA POSICION
        System.out.println("Comilla simple: \'" + nombre + "\'");
        System.out.println(" Comilla doble: \"" + nombre + "\"");


      System.out.println("Saludos");   //ln -> nueva linea
      System.out.print("Adios"); //cuando se imprima la siguiente linea no hara el salto de linea porque no es println
      System.out.println("hasta luego"); // se imprimira a lado de adios asi: adioshastaluego porque no tiene el salto de linea
        
    }
    
}

``````