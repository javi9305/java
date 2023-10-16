  
  `````` java
  
   public static void main(String[] args) {

  //Creacion de un objeto tipo Persona    
        //Para asignarle un valor a esta variable necesitamos instanciar nuestra clase persona.
        Persona persona1;
        
        //Instanciando (creando) un objeto de la clase Persona
        /*
        - va a crear un objeto de nuestra clase Persona. sin embargo necesitamos asignarlo a nuestra variable persona1 de lo contrario no vamos a poder acceder a este objeto.
        
        - Esta linea lo que va a hacer es lo siguiente:
          De nuestra plantilla Persona, la palabra new va a crear un nuevo objeto
          de tipo Persona, pero necesitamos que nuestra variable persona1
          apunte al objeto que se acaba de crear y para que pueda acceder al objeto
          que se acaba de crear entonces hacemos lo siguiente:

          persona1 = new Persona();

          persona1 debe recibir el valor donde se ha creado este objeto,
          en el lado derecho lo que estamos haciendo es que estamos creando el objeto
          y el valor donde se ha creado este objeto entonces se le proporciona a la
          persona1 para que se pueda acceder al objeto que se creado.
        
        */
        persona1 = new Persona(); 

   }
``````

Asi se representa persona1 = new Persona(), **ver imagen 1.1**

![dibujoobjeto](/imagenesjava/dibujoobjeto.png "dibujoobjeto")

**imagen 1.1**


`````` java
 //Accedemos al objeto Persona, y llamamos al metodo desplegarNombres
         persona1.desplegarNombres();
        
         //Modificamos los valores de los atributos del objeto Persona
         //Ojo: modificar los valores asi no es una buena practica
        persona1.nombre = "juan";
        persona1.apellido = "perez";

        //Volvemos a imprimir los valores
        System.out.println("");
        persona1.desplegarNombres();



``````

lo que hizo la variable persona1 es que accedio a nuestro objeto y los modificó
por ello es que cuando se mando a llamar el metodo desplegarNombres()
lo que imprime son los atributos del objeto y no los valores de la clase.
Basicamente lo que se hace es que la plantilla de Persona crea un
objeto a su semejanza es decir con los atributos y metodos que hemos definido
en nuestra plantilla pero los valores no se estan modificando en nuestra
clase, aqui unicamente tenemos la plantilla sino los valores se estan modificando
en el objeto que se ha creado. **Ver imagen 1.2**


![dibujoobjeto2](/imagenesjava/dibujoobjeto2.png "dibujoobjeto2")


**Imagen 1.2**

**Nota:** Cada que veamos la palabra new es porque se esta creando un nuevo objeto en memoria.

`````` java
//Creacion de un segundo objeto de tipo Persona
        
        Persona persona2 = new Persona();
        
        
        persona2.desplegarNombres();
        
        persona2.nombre = "Karla";
        persona2.apellido = "Lara";
        
        System.out.println(" ");
        
        persona2.desplegarNombres();

``````


Si creamos mas objetos entonces cada uno de los objetos tiene acceso a sus propios atributos,
asi que los valores no porque modifiquemos los valores del objeto que se ha creado persona1,
cada uno de los objetos va a tener sus propios valores. **ver imagen 1.3**

![dibujoobjeto3](/imagenesjava/dibujoobjeto3.png "dibujoobjeto3")


**imagen 1.3**

el primer objeto tiene los valores de juan perez y el segundo objeto tiene el valor de karla lara, y observamos que la plantilla no se altera, esta contiene la base o la estructura para crear estos objetos, pero la plantilla no se modifica, lo que se modifica son los valores de los objetos que se han creado.
**ver imagen 1.4**

![dibujoobjeto4](/imagenesjava/dibujoobjeto4.png "dibujoobjeto4")


**imagen 1.4**



 estos objetos se depositan en algun lugar de la memoria, por ejemplo si ponemos un valor hexadecimal que es la direccion de memoria 0x333, este es el valor de memoria donde se encuentra el objeto persona, a esta direccion de memoria se le conoce como referencia del objeto, y realmente lo que almacena la variable persona1 es el valor de la referencia de la memoria del objeto.

 asi que de esta manera la variable persona1 apunta al objeto que se ha creado en esta direccion de memoria 
 (0 x333). y cada vez que utilizamos la palabra reservada new  es que se crea un objeto y se le asigna una referencia en memoria  dinamicamente, esto lo hace automaticamente el compilador de java o la maquina virtual de java y la segunda vez que se mando a llamar la palabra new  y se creo este segundo objeto y se deposito por ejemplo en la referencia de memoria en 0x444.

 las variables almacenan la direccion de memoria de los objetos, esta caracteristica en otros lenguajes se le conoce como apuntadores.

cada vez que creamos un objeto, se le asigna una referencia en memoria y son las variables que almacenan estas referencia, por lo tanto estas variables apuntan al objeto. **ver imagen 1.5**


![dibujoobjeto5](/imagenesjava/dibujoobjeto5.png "dibujoobjeto5")


**Imagen 1.5**