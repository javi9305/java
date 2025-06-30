

# Explicando la clase scanner

`````` java

public class EjercicioScaner {

    //Metodo principal main
    public static void main(String[] args) {
        
        System.out.println("Escribe tu nombre"); 
         //in nos va a permitir acceder a la consola.
         //Se crea un objeto llamado consola de tipo Scanner (clase Scanner).
        Scanner consola = new Scanner(System.in);

        /*
        consola.nextline lo que a hacer es que se va a detener hasta que el usuario escriba 
        una información y una vez que escribe la información y da enter entonces el valor 
        que se escribe se asigna a usuario.
        
        con esta linea de manera dinamica  estamos recuperado el valor de juan  
        utilizando el metodo nextline, este metodo nextline lo que hace es  detener 
        la ejecución de nuestro programa para esperar que el usuario escriba una información 
        y una vez que da enter el resultado se asigna a usuario. */
       
        //nextLine lee una linea completa de la consola.
        var usuario = consola.nextLine(); 
        //Muestra el nombre escrito por el usuario. (concatenacion)
        System.out.println("Usuario = " + usuario);
        
        //Se visualiza que se debera escribir un titulo en la consola.
        System.out.println("Escribe el titulo:"); 
        //Se pide al usuario  que escriba un titulo en la consola y el valor escrito es almaceado en la variable titulo.
        var titulo = consola.nextLine(); 
        //Muestra el titulo y nombre escrito por el usuario. (concatenacion)
        System.out.println("Resultado: " + titulo + " " + usuario);
    }
    
}
``````