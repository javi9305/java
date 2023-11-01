
Este codigo es sin usar el encapsulamiento

`````` java
public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona = new Persona("Juan", 500, false);
    
        //No es recomendable acceder directamente a los atributos de la clase Persona si estamos en otra clase.
        //El acceder directamente a los atributos solo debe ser dentro de la misma clase.
        System.out.println("nombre persona: " +persona.nombre);
    }
}

``````

Usando el encapsulamiento

`````` java


public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona = new Persona("Juan", 5000, false);
    
        /*
            No es recomendable acceder directamente a los atributos de la
            clase Persona si estamos en otra clase en este caso PruebaPersona.
            por ejemplo hacer esto Persona.nombre  */
        
        System.out.println("nombre persona: " +persona.getNombre());
        System.out.println("sueldo persona:" + persona.getSueldo());
        System.out.println("¿Persona borrada?" + persona.isEliminado());
        
        persona.setNombre("Carlos");
        persona.setSueldo(3000);
        persona.setEliminado(true);
        
        System.out.println("nombre persona:"+ persona.getNombre());
        System.out.println("sueldo persona:" + persona.getSueldo());
        System.out.println("¿Persona borrada?" + persona.isEliminado());
    }
}

`````` 

Explicacion de codigo

![encapsulamiento](/imagenesjava/encapsulamiento.png "encapsulamiento")



Se crea un objeto de tipo Persona pero lo que estamos haciendo internamente es que el atributo de nombre ya es de tipo privado, así que ya no lo podemos acceder desde otras clases directamente sino ahora lo que tenemos que hacer es acceder a través de método get(para obtener el valor del atributo) y set(modificar el valor del atributo) para el atributo respectivo. Ya no podemos acceder directamente al atributo, sino que ahora va a hacer a través de los métodos get o set.
En este caso como estamos en la clase PruebaPersona, entonces la variable persona apunta al objeto persona, pero ya no puede acceder directamente al atributo de nombre, sino que ahora tiene que utilizar el método getNombre para acceder indirectamente al atributo de nombre.
