### Arreglo de tipo object

Se va a reservar espacio en memoria para 4 objetos de tipo Persona, así que en memoria vamos a tener lo siguiente:

![arreglopersona1](/imagenesjava/arreglopersona1.png "arreglopersona1")



Tenemos nuestra memoria y estamos reservando espacio para 4 objetos de tipo Persona, sin embargo, internamente lo que va a suceder es lo siguiente:

![arreglopersona2](/imagenesjava/arreglopersona2.png "arreglopersona2")


- Lo que estamos declarando son objetos de tipo object, asi que cada uno de los elementos del arreglo lo que va a almacenar es una referencia a un objeto de tipo object, esto va a suceder hasta que se le asigne la referencia, asi que en este arreglo estamos definiendo que este arreglo va a almacenar referencias de tipo Persona.

- El valor por default si no indicamos nada sera de null.
 
- Si por ejemplo le asignamos una referencia al índice 0, lo que va a suceder es que en memoria va a estar apuntando una referencia en memoria donde se va a crear un objeto de tipo persona, en este caso se va a crear un objeto de tipo persona e internamente contiene el valor de nombre, ya que la clase persona contiene el atributo de nombre y así sucesivamente cada uno de estos índices va a estar apuntando a un objeto en memoria de tipo persona, no sabemos exactamente donde se van a almacenar pero por ello estos índices van a estar apuntando a una referencia en memoria donde se van a estar creando estos objetos.