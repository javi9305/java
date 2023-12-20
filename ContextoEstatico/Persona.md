

`````` java

public class Persona {
    /*
     el idPersona va a almacenar el valor del id que le vamos a asignar al
      objeto de tipo Persona cada que creemos un objeto.
    
    por cada objeto creado va a contener diferentes valores en cada atributo
    que no es estatico pero si el atributo es estatico se asocia con la clase.
    
    Por lo tanto los objetos si acceden al atributo estatico, todos los 
    objetos van a poder acceder al mismo valor, ya que este valor (contadorPersonas)se asocia
    con la clase/plantilla y no con los objetos.
    */
    private int idPersona; //se asocia con un objeto (instancia)
     private String nombre; //se asocia con un objeto (instancia)
    
    private static int contadorPersonas; //se asocia con la clase
    
    public Persona(String nombre){
     this.idPersona = ++contadorPersonas;
     this.nombre = nombre;   
    }
    
    public int getIdPersona(){
     return this.idPersona;
    }
    
    /*
    Como el constructor ya inicializo el valor idPersona podriamos omitir este metodo set
     ponemos el metodo set en comentarios debido a que el valor idPersona se va a modificar
    a traves del constructor y no a traves del metodo set, esto quiere decir que no siempre
    debemos generar el metodo set o get sino que dependiendo de lo que necesitemos  es que se pueden
    agregar ciertos metodos.
    */ 
//    public void setIdPersona(int idPersona){
//     this.idPersona = idPersona;
//    }
    
    public String getNombre(){
      return this.nombre;
    }
    
    public void setNombre(String nombre){
      this.nombre = nombre;
    }
    
    //Para saber cuantos objetos de tipo persona se han creado.
    /*
    Ya que cada vez que se crea un objeto persona se esta incrementando la variable contadorPersonas,
    ya que se asocia con la clase. el metodo va a hacer de tipo static ya que lo que va a utilizar 
    es nuestra variable estatica contadorPersonas.
    */
    public static int getContadorPersonas(){
     return contadorPersonas;
    }
    
    @Override
    public String toString(){
     return "idPersona: " + idPersona + ", Nombre: " + nombre + ", contadorPersonas: " + contadorPersonas;
    }
  
}

`````` 

Explicacion de codigo

![contextoestatico1](/imagenesjava/contextoestatico1.png "contextoestatico1")

Si queremos acceder al atributo estático usando this, veremos que no es posible, ya que, al colocar el punto, no muestra el atributo contadorPersonas, esto debido a que el operador this se asocia con el contexto dinámico y los atributos y métodos estáticos se asocian con la clase, con el contexto estático.
Lo que significa es lo siguiente:
Nuestra clase Persona, primero se debe levantar en memoria para que pueda ser utilizada, así que en este momento estamos en el contexto estático y una vez que esta clase ya se levanto en memoria, podemos crear objetos y estos objetos, entonces ya estamos en contexto dinámico.
Por lo tanto, los objetos si pueden acceder al contexto estático pero el contexto estático no puede acceder al contexto dinámico ya que aun no ha sido creado. Así que en este sentido el contexto estático no puede acceder al contexto dinámico pero el contexto dinámico si puede acceder al contexto estático, ya que una vez se ha cargado la clase en memoria, entonces los objetos si pueden acceder a la clase es decir al contexto estático.


![contextoestatico2](/imagenesjava/contextoestatico2.png "contextoestatico2")


Y por lo tanto los métodos o atributos estáticos que se declaren en la clase Persona, se van a asociar con la clase, por lo tanto el atributo de contadorPersona, se va a asociar con nuestra clase y los objetos lo que van a hacer es acceder a contadorPersona, todos los objetos que se creen van a acceder al mismo valor es decir a contadorPersona, a diferencia de los atributos no estáticos que son idPersona y nombre, esos se asocian con los objetos y cada objeto va a tener su propio valor, pero en particular los atributos estáticos van a compartir su valor con todos los objetos que se creen de tipo persona. 
Y por ello es que el operador this ,recordemos que el operador this es un apuntador al objeto que se esté ejecutando en dicho momento pero quiere decir que ya debimos de haber creado el objeto y por lo tanto estamos en el contexto dinámico, pero si estamos en el contexto estático aun no se han creado objetos, ya que solamente se ha cargado la clase en memoria, esto quiere decir que el operador this no puede acceder al contexto estático y por lo tanto this no puede utilizar los atributos o métodos estáticos.



