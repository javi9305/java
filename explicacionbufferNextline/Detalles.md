# Clase Scanner para leer datos en consola 

Para utilizar la clase Scanner en una clase debemos hacer lo siguiente:

1. En las primeras lineas de la clase debemos escribir lo siguiente:

 import java.util.Scanner 

lo que significa, importame la clase Scanner que esta en el paquete java.util para que pueda utilizarla.

2. Creamos un objeto de la clase Scanner asociado al dispositivo de entrada que en este caso
sera el teclado y se representa con System.in; aunque pueden haber otros dispositivos de entrada.

Scanner consola = new Scanner(System.in);

3. Ahora se muestra algunos metodos de la clase Scanner para leer datos desde el teclado:

![metodosdelaclasescanner](/imagenesjava/metodosdelaclasescanner.png "metodosdelaclasescanner")


4. Ahora vamos a mostrar como se puede utilizar el metodo nextInt().

int numero;
System.out.println("Introduce un número entero: ")
numero = consola.nextInt(); //Asigna a la variable numero, el numero entero introducido por teclado.


dependiendo del tipo de dato,se usa algun metodo por ejemplo si necesitamos ingresar por teclado
un dato de tipo String usamos el metodo nextLine().


Asi se veria un programa con lectura de datos con la clase Scanner


import java.util.Scanner

public class PruebaScanner {
    
    public static void main(String[] args){
    
        Scanner consola = new Scanner(System.in) //creamos un objeto Scanner.
 
        //Declaramos las variables a ocupar.
        int numero;
        String nombre;

        System.out.println("Introduce un nombre");
        nombre = consola.nextLine();

        System.out.println("Introduce un numero")
        numero = consola.nextInt();


        System.out.println("El nombre es: " + nombre)
        System.out.println("El numero es: " + numero)
    }



}



Si el valor introducido por teclado no es del tipo esperado, se producira un error llamado: inputMismatchException.



Funcionamiento interno de la clase Scanner


![scannerinterno](/imagenesjava/scannerinterno.png "scannerinterno")



Para mas información de la clase scanner y como vaciar el buffer,visitar la pagina:

[puntocomnoesunlenguaje.blogspot.com/2012/08/java-scanner.html](https://puntocomnoesunlenguaje.blogspot.com/2012/08/java-scanner.html)