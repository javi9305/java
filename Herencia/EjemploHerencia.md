`````` java

   public static void main(String[] args) {
        /*Tambien se pueden pasar los datos con el contructor correspondiente 
          Empleado empleado1 = new Empleado("Juan", 'm',24,"Av.10 de julio",5000);
        */
       
      Empleado empleado1 = new Empleado("Juan",5000);
       empleado1.setEdad(28); //Metodo es heredado de la clase Persona
      empleado1.setGenero('M');
      empleado1.setDireccion("Lomas 232");
      
      System.out.println(empleado1);
      
      Cliente cliente1 = new Cliente(new Date(),true);
        cliente1.setNombre("Karla");
        System.out.println(cliente1);
    }


``````

Explicacion del codigo

En este momento ya se ha creado un **objeto de tipo empleado en memoria**, pero debido a que hemos definido **el método toString en la clase empleado ya no observamos la referencia en memoria, sino que ahora observamos los valores del método toString.**


![herencia1](/imagenesjava/herencia1.png "herencia1")


Tenemos un objeto de tipo empleado, pero internamente **tenemos las características de la clase Padre Persona** y a su vez esta clase persona tiene **internamente las características** de la clase Object, así que este es el orden de creación de los objetos, se crea nuestro objeto empleado, pero se debe terminar de inicializar el objeto Persona y a su vez el objeto persona manda a llamar al constructor de la clase Object y ahí donde se crea el espacio en memoria (se asigna la referencia en memoria).

![herencia2](/imagenesjava/herencia2.png "herencia2")

 y termina de asignar las características de la clase padre, la clase persona y finalmente termina de asignar las características de la clase empleado.
Pero es un solo objeto en memoria que internamente tiene las características de la clase Padre.



**nota:** Empleado tiene dentro a la clase Padre Persona y Persona tiene dentro a la clase Object