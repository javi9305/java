
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



Usando el metodo toString para mejorar el codigo


Si nos damos cuenta cada vez que queremos imprimir los valores del objeto persona, estamos imprimiendo demasiadas lineas en consola, asi que con cada cambio que le hacemos al objeto, estamos mandando a llamar 3 veces la impresion la salida(a esto nos referimos con 3 veces: persona.getNombre, persona.getSueldo,persona.isEliminado).Para mejorar esto podemos hacer uso del metodo toString.




``````java

public class PruebaPersona {
    public static void main(String[] args) {
        Persona persona = new Persona("Juan", 5000, false);
    
      
        /*
        Debido a que el metodo toString es muy utilizado en java el metodo 
         println en automatico al poner una referencia de un objeto en java
         manda a llamar en automatico al metodo toString(), podemos agregar
        el metodo o no sin embargo el resultado es el mismo.
        
        System.out.println("persona:" + persona.toString());
        */
         System.out.println("persona:" + persona);
        
        persona.setNombre("Carlos");
        persona.setSueldo(3000);
        persona.setEliminado(true);
        
        System.out.println("persona:" + persona);
    }
}

``````