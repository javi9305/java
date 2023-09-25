# Creando una clase

![clase1](/imagenesjava/clase1.png "clase1")

![dependencia](/imagenesjava/dependencia.png "dependencia")

![raiz](/imagenesjava/raiz1.png "raiz")


**Java with maven**  maven es una tecnologia que nos va a servir para administrar mas facilmente las librerias

que se van a utilizar cuando se trabaja con java.

**Java with gradle**  tambien permite administrar librerias.










`````` java

public class HolaMundo {
    //main sirve para ejecutar el codigo
    //public -> Modificador de acceso que nos permite acceder a este metodo desde otras clases java.
    //static -> Nos permite ejecutar el metodo main sin necesidad de crear un objeto de esta clase.
    // void -> este metodo no va a regresar ninguna información, ya que los metodos podrian regresar información o no. en este caso como no va a regresar información se usa void (vacio o que no regresa ningun tipo de información).
    //main -> la palabra main se selecciono para indicar que este metodo va a ser el metodo principal y se utiliza por el compilador de java para poder ejecutar esta clase.
    // String -> indicamos los argumentos que va a recibir nuestro metodo, ya que podria  recibir información este metodo cuando es llamado, String es una clase que se utiliza
    //para trabajar con cadenas, asi que este tipo de datos nos permite almacenar cadenas.
    //args -> es el nombre de nuestra variable.
    // [] - > estos corchetes estan indicando que esto es un arreglo (los corchetes puede ir de lado derecho o de lado izquierdo)
    //todo lo que este dentro de estas llaves {} se conoce como cuerpo del metodo.

    public static void main(String[] args) {
        System.out.println("Hola mundo desde java"); //Imprime un mensaje en la consola.
    }
}


``````