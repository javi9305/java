# La importancia de las variables
`````` java

// sin usar una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        
   //Imprimira 3 veces la palabra saludos!!     
   System.out.println("Saludos!!!")
   System.out.println("Saludos!!!")
   System.out.println("Saludos!!!")

   //si se quisiera hacer una modificación se tendria que hacer en cada linea.
   //esto no es lo mas práctico si queremos realizar cambios de una sola vez.
   System.out.println("Saludos");
   System.out.println("Saludos");
   System.out.println("Saludos");

    }

``````


`````` java

// Usando una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        //Agregar la cadena de saludos en una variable
           String saludar = "saludos";

 //en lugar de usar la cadena vamos a utilizar la variable y se imprimira lo que contiene la variable saludar
   System.out.println(saludar);
   System.out.println(saludar);
   System.out.println(saludar);

    }

``````

`````` java

// cambiando contenido de una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        
           String saludar = "saludos desde java"; //si quisieramos hacer un cambio solo lo hariamos en un solo lugar en este caso la variable saludar.

 //este cambio se replicara en la variable saludar.
   System.out.println(saludar);
   System.out.println(saludar);
   System.out.println(saludar);

    }

``````