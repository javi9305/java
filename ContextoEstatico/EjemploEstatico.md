
`````` java

public class EjemploEstatico {

    public static void main(String[] args) {
        Persona persona1 = new Persona("Juan");
        System.out.println(persona1);
        
        Persona persona2 = new Persona("Karla");
        System.out.println(persona2);
        
        //no se usa ningun objeto, sino usamos el nombre de la clase.
        System.out.println("contadorPersonas: " + Persona.getContadorPersonas());
    }
}

``````


Explicacion de codigo


![contextoestatico3](/imagenesjava/contextoestatico3.png "contextoestatico3")


¿Cuándo se carga la clase Persona en memoria?

La primera vez que lee una línea de código y necesita de la clase persona, en este caso la primera vez que ubica la clase Persona es cuando se carga en memoria. Así que en ese momento es cuando todo el contexto estático se inicia, ya que la clase Persona se carga en memoria y todo lo que sea referente al contexto estático se empieza a ejecutar, posteriormente cuando ya empiezan las siguientes líneas de código y empezamos a ejecutar la creación de objetos, entonces ya tenemos el contexto dinámico y es cuando creamos los objetos y se crean las variables que apuntan a estos objetos.(p1 y p2) Y cada uno de los objetos va a utilizar el contadorPersonas pero recordemos que es un atributo estático. Así que la variable contadorPersonas se asocia con la clase ya que es un atributo estático y por lo tanto cada vez que modifiquemos este valor por ejemplo el valor de 1, todos los objetos van a ver este mismo valor, si se cambia a 2, todos los objetos van a ver ese mismo valor. Si contadorPersonas no fuera estático entonces en lugar de asociarse con la clase, se asociaría con cada uno de los objetos y cada objeto tendría sus propios valores es decir contadorPersonas se inicializaría con cada creación de cada objeto.