``````java


public class SobrecargaConstructores {
    public static void main(String[] args) {
        Persona persona1 = new Persona("Juan",25);
        System.out.println("persona" + persona1);
        
        Empleado empleado1 = new Empleado("Maria",30,3000);
        System.out.println("empleado1 = " + empleado1);
    }
  
}

``````


explicacion de la creacion del objeto en una herencia.


Podemos observar que el orden de nuestras clases (la jerarquía de clases) tenemos la clase Object, como la clase padre de todas las clases, posteriormente tenemos la clase Persona que hereda de la clase Object y tenemos nuestra clase Empleado que hereda de la clase Persona.


![sobrecarga1](/imagenesjava/sobrecarga1.png "sobrecarga1")


Entonces cuando creamos el objeto de tipo Empleado llamado empleado1, lo que tiene que hacer en primer lugar es mandar a llamar los constructores, en este caso de la clase Persona y posteriormente al de la clase Object como se ve en la imagen.

![sobrecarga2](/imagenesjava/sobrecarga2.png "sobrecarga2")


Y para terminar de crear el objeto, ahora empieza el trabajo hacia abajo, vamos a empezar a regresar de la clase Object a Persona, de la clase Persona a la clase Empleado y finalmente regresa la referencia a la variable empleado1. Y este es el orden de creación del objeto, incluyendo el orden de llamada de los constructores.

![sobrecarga3](/imagenesjava/sobrecarga3.png "sobrecarga3")