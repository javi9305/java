

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
     Ya que cada vez que se crea un objeto persona se esta incrementando la variable contadorPersonas, ya que se asocia con la clase.
     el metodo va a hacer de tipo static ya que lo que va a utilizar es nuestra variable estatica contadorPersonas.
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


![contextoestatico3](/imagenesjava/contextoestatico3.png "contextoestatico3")


¿Cuándo se carga la clase Persona en memoria?
La primera vez que lee una línea de código y necesita de la clase persona, en este caso la primera vez que ubica la clase Persona es cuando se carga en memoria. Así que en ese momento es cuando todo el contexto estático se inicia, ya que la clase Persona se carga en memoria y todo lo que sea referente al contexto estático se empieza a ejecutar, posteriormente cuando ya empiezan las siguientes líneas de código y empezamos a ejecutar la creación de objetos, entonces ya tenemos el contexto dinámico y es cuando creamos los objetos y se crean las variables que apuntan a estos objetos.(p1 y p2) Y cada uno de los objetos va a utilizar el contadorPersonas pero recordemos que es un atributo estático. Así que la variable contadorPersonas se asocia con la clase ya que es un atributo estático y por lo tanto cada vez que modifiquemos este valor por ejemplo el valor de 1, todos los objetos van a ver este mismo valor, si se cambia a 2, todos los objetos van a ver ese mismo valor. Si contadorPersonas no fuera estático entonces en lugar de asociarse con la clase, se asociaría con cada uno de los objetos y cada objeto tendría sus propios valores es decir contadorPersonas se inicializaría con cada creación de cada objeto.
