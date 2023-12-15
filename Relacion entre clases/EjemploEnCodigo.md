## Implementacion en codigo.

![celular](/imagenesjava/celular6.png)


### Clase Bateria.


![clasebateria](/imagenesjava/clasebateria.png)

### Clase Chip.


![clasechip](/imagenesjava/clasechip.png)

### Clase SmartPhone.

![clasecelular](/imagenesjava/clasecelular.png)



El atributo bateria es de la clase Bateria, que es el atributo que hace la relacion de composicion con la clase Bateria

Un arreglo de chips, el cual hace una relacion de agregacion con la clase Chip.


### Consideraciones para la implementacion de la composicion: En el constructor.

![constructorcel](/imagenesjava/constructorcel.png)

En el constructor podemos ver que recibimos un String modelo y otros 2 atributos para crear una bateria.

Recordemos que una regla de la composicion es que:  si se elimina la clase todo, tambien debe eliminarse la clase parte, entonces es recomendable instanciar
el objeto bateria dentro del constructor, es por eso que recibimos los parametros de bateria mediante el constructor de la clase SmartPhone.

### Consideraciones para la implementacion de la agregacion: En el constructor.

Cuando hablamos de agregacion, el atributo que relaciona con agregacion en este caso chips debe empezar en cero, por eso colocamos nroChips en cero e inicializar un arreglo de chips, pero sin ningun dato.

![constructoragregacion](/imagenesjava/constructoragregacion.png)


### En los metodos

Cuando hablamos de agregacion usualmente tendriamos un metodo para agregar una cantidad de partes, en este caso nuestro metodo se llama agregarChip, que recibe un Chip como parametro y lo agregamos en nuestro arreglo de chips. 


![metodosarreglo](/imagenesjava/metodosarreglo.png)


### Creacion de objetos en la clase main

![creacionobjeto](/imagenesjava/creacionobjeto.png)

### Agregacion vs Composicion

![tablas](/imagenesjava/tablas.png)


[Video de explicacion](https://www.youtube.com/watch?v=U9-iM-gA7-E/ "Agregacion y Composicion en POO")