

``````java

public class SobrecargaMetodos {
    public static void main(String[] args) {
        /*Aqui lo interesante es, cual de los metodos sumar se manda a llamar
         dependiendo de los argumentos que enviemos al metodo sumar*/
        System.out.println("Resultado 1:" + Operaciones.sumar(3, 4));
        /*Como uno de sus argumentos fue entero, ya no se puede mandar a llamar el
         metodo que contiene los argumentos enteros, ya que este metodo contiene un double(el 2.0).
        
          No se puede mandar a llamar el metodo sumar(int,int) porque un double no se puede almacenar en un int,
          ya que un double tiene 64 bits y un int solo tiene 32 bits.
        */
        
        
     /*Como se realizo cambios, y agregamos ahora el metodo(double,int) ahora
       se manda a llamar este metodo ya que soporta el tipo double y el tipo int en este orden*/
        System.out.println("Resultado 2:" + Operaciones.sumar(2.0, 4));
        
        //invertimos el orden de los argumentos
        /*
        Se mandaria a llamar el metodo sumar(int a, double b) ya que 
        un tipo long se puede almacenar en un float, esto es porque no tenemos
        el metodo sobrecargado con el tipo long, y como no existe un metodo
         con el tipo float, entonces busca un metodo con tipo double.
        
        se estaria haciendo un upcasting o una conversion hacia arriba de manera automatica, va a buscar
        el tipo que soporte de mejor manera almacenar su valor, en este caso
        si hubiera tipo long, buscaria utilizar un metodo con un argumento de tipo long,
        como no existe entonces busca el argumento de tipo float y como tampoco
        existe busca entonces el tipo double.
        
        */
        System.out.println("Resultado 3:" + Operaciones.sumar(3, 5L));
        
        
        
        /*
        Se puede mandar a llamar 2 metodos el sumar(double a, double b) o
        el sumar(double a, int b), java lo que hace es tomar el que tiene
        menor cantidad de bits, que en este caso es el int.
        
        Esto se debe a que el char empieza su conversion hacia arriba y al no
        encontrar un tipo char que lo pueda almacenar, entonces busca el siguiente
        tipo, en este caso el tipo entero.
        */
        
        System.out.println("Resultado 4:" + Operaciones.sumar(3F, 'A'));
    }
}


``````


Explicacion del ultimo método.


En primer lugar tenemos el tipo byte con 8 bits, posteriormente tenemos el tipo short y el tipo char con 16 bits, posteriormente estos se pueden convertir a un tipo entero que tiene 32 bits, posteriormente este se puede convertir en un tipo long de manera automática que tiene 64 bits, el long se puede almacenar a un tipo flotante y aunque tiene menos bits maneja la notación exponencial, por lo tanto un valor de tipo long se puede almacenar en un tipo float debido a que maneja la notación exponencial y puede almacenar números mas grandes que el tipo long y finalmente el tipo double tiene 64 bits con notación exponencial.


![sobrecargametodos1](/imagenesjava/sobrecargametodos1.png "sobrecargametodos1")

En el caso el argumento long del método sumar (3, 5L), busca un tipo Long para almacenar, pero como no existe esta firma de método, entonces busca un tipo float, pero como no existe finalmente busca el tipo double, así que el método que se mando a llamar es el que recibe un entero y un double.
Esto es lo que sucede el tipo long busca asignarse a un tipo float, pero como no existe busca asignarlo a un tipo double.


![sobrecargametodos2](/imagenesjava/sobrecargametodos2.png "sobrecargametodos2")