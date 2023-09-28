

# Explicando la clase scanner

`````` java

public class EjercicioScaner {

    //Metodo principal main
    public static void main(String[] args) {
        
        System.out.println("Escribe tu nombre"); //Se visualiza que se debera escribir un nombre en la consola
         //in nos va a permitir acceder a la consola.
        Scanner consola = new Scanner(System.in);//Se crea un objeto llamado consola de tipo Scanner (clase Scanner).

        /*
        consola.nextline lo que a hacer es que se va a detener hasta que el usuario escriba una información y una vez que escribe la información y da enter entonces el valor que se escribe se asigna a usuario.
        
        con esta linea de manera dinamica  estamos recuperado el valor de juan  utilizando el metodo nextline, este metodo nextline lo que hace es  detener la ejecución de nuestro programa para
        esperar que el usuario escriba una información  y una vez que da enter el resultado se asigna a usuario. */
       
       
        var usuario = consola.nextLine(); //nextLine lee una linea completa de la consola.

        System.out.println("Usuario = " + usuario);//Muestra el nombre escrito por el usuario. (concatenacion)
        
        System.out.println("Escribe el titulo:"); //Se visualiza que se debera escribir un titulo en la consola.
        var titulo = consola.nextLine(); //Se pide al usuario  que escriba un titulo en la consola y el valor escrito es almaceado en la variable titulo.
        System.out.println("Resultado: " + titulo + " " + usuario);//Muestra el titulo y nombre escrito por el usuario. (concatenacion)
    }
    
}
``````