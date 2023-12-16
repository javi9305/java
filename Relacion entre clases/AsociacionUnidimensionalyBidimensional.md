### ¿Cuando se da una asociacion ?

una asociacion se da cuando tengo una clase que tiene atributos de tipo  otra clase, por ejemplo cuando yo digo que una cuenta tiene dinero, una cuenta tiene un titular que es un cliente.

Por eso la asociacion se le conoce con el nombre de "relacion de tipo" o "Tiene un"

![claseasociacion](/imagenesjava/claseasociacion.png)

### ¿Como represento una asociacion?

se representa con una linea continua y una flecha indicando como la leo, que quiere decir esto:

si tengo una linea sola, es bidireccional es decir la puedo leer de un lado o el otro y si tiene una direccion indicando la direccion en la que la tengo que leer.


![asociacionbidireccional](/imagenesjava/asociacionbidireccional.png)



Cuenta esta asociada con dinero y con cliente, si ponemos el foco entre cuenta y dinero, decimos que cuenta tambien tiene un atributo de tipo dinero, y la leo de cuenta a dinero, por que la flecha va de cuenta a dinero.



![diagramacuenta](/imagenesjava/diagramacuenta.png)




Que quiere decir esto, que si tengo la asocacion no es necesario tener el atributo Dinero dinero, ya me lo esta diciendo el diagrama UML y ademas ya tiene un nombre que es balance.

![diagramacuenta1](/imagenesjava/diagramacuenta1.png)



Ahora la clase Cuenta tiene un atributo de tipo Cliente llamado titular, ademas es bidireccional, entonces esto me esta diciendo que si tomo una cuenta tiene un titular y si tomo un cliente tambien tiene una cuenta de tipo Cuenta, se puede leer de los 2 lados es decir si me paro en la clase Cuenta, tengo un atributo de tipo Cliente y si me paro del lado del Cliente, tengo un atributo de tipo Cuenta.

![diagramacuenta2](/imagenesjava/diagramacuenta2.png)