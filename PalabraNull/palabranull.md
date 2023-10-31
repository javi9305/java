


`````` java

public class PalabraNull {

    public static void main(String[] args) {
        Persona persona1 = new Persona("Juan");
        System.out.println("persona1: " + persona1.obtenerNombre());
        
        Persona persona2 = persona1;
        System.out.println("persona2: " + persona2.obtenerNombre());
        
        //utilizaremos la palabra null para indicar que la persona1 ya no va a apuntar al objeto
        persona1 = null;
        
        if(persona1 != null)
         System.out.println("persona1: " + persona1.obtenerNombre());
        else
            System.out.println("la variable persona1 no apunta a ningun objeto");
        
       
        /*
        este metodo va a escanear todo los objetos que se han creado en memoria
        y los va a quitar de la memoria, sin embargo este metodo unicamente
        podemos planificarlo, podemos hacer la llamada, pero esto no garantiza
        que se ejecute el recolector de basura(garbage collector, solo podemos
         planificar la llamada para recolectar objetos que ya no estan haciendo
         apuntado por ninguna variable), ya que es un
       proceso muy pesado y unicamente se va a ejecutar en cuanto le sea posible
         a la maquina virtual, ya que la maquina virtual es quien se va a 
         encargar de ejecutar el recolector de basura 

        System.gc(); 

       si mandamos a llamar el metodo garbage collector entonces no significa
       que se va a ejecutar de manera inmediata sino hasta que la maquina virtual
      pueda ejecutar este proceso es que va a ejecutarlo y se van a eliminar
      de la memoria los objetos que ya no estan siendo  referenciados por
      ninguna variable. */
    }
}

class Persona{
   String nombre;
   
   Persona(String nombre){
     this.nombre = nombre;
   }
   
   public String obtenerNombre(){
       return this.nombre;
   }
   

}

``````