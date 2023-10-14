# ¿Cuales son las caracteristicas de una clase?

* Una clases es una plantilla.
* Posee un nombre.
* Posee atributos y metodos.
* Un objeto es una instancia de una clase.

# ¿Por qué una clase es fundamental en java?

porque una **clase define la naturaleza de un objeto**, por lo tanto una clase provee las bases de la programación
orientada a objetos. Asi que cualquier concepto que se vaya a implementar en java está envuelto en una clase.

# ¿Cuál es uno de los punto más importantes de una clase?

una clase **genera un nuevo tipo de datos** en java. Una vez definido este tipo de datos, entonces lo podemos 
**utilizar para crear objetos del tipo previamente definido.**

# En terminos generales, ¿Que es una clase?

Es una plantilla para poder crear objetos es decir podremod generar objetos (instancias) para que puedan
ser finalmente utilizados los nuevos tipos de datos de un programa.

# ¿Con que otro nombre se le conoce a una instancia de una clase?

Objeto.

# ¿Cuáles son los pasos para crear una clase?

* Definir el nombre de la clase, anteponiendo la palabra reservada **class**
* Definir los atributos o variables de nuestra clase. Tambien conocidas como **Variables de instancia**
* Definir los métodos de nuestra clase, estos contienen la funcionabilidad y objetivo de ser de nuestra clase.

# ¿Debemos definir todos los atributos y/o métodos desde un inicio a nuestra clase, o debemos esperar a que las necesidades o requerimientos vayan complementando el código de la misma?

Depende muchas ocasiones de la metodologia de desarrollo de software que estemos utilizando, pero en general, agregamos los métodos que surjan del analisis de nuestro sistema.
Asi que posiblemente la clase tendrá más métodos y atributos que vayamos a utilizar en un inicio, pero nuestra clase o plantilla estará lista para soportar
futuros cambios en nuestro sistema. Por eso es que en ocasiones encontraremos atributos o métodos en nuestras clases que son poco o nunca utilizamos al momento de
crear objetos de dichas plantillas.

# ¿Qué es lo importante que se debe recordar de una clase?

Es importante recordar que al definir una clase, solo **estamos definiendo una plantilla con la que vamos a trabajar,** pero para poder usar esa plantilla
necesitamos **crear objetos a partir de esa plantilla.** Definir la clase **no crear un objeto en automático, tenemos que crearlos.**


Por ejemplo:


![ejemploclase](/imagenesjava/ejemploclase.png "ejemploclase")


# ¿Por medio de que se extrae la información del mundo real?

Atributos y métodos.

# ¿Cómo debe ser los nombres de una clase?

lo ideal es que los nombres de las clases, métodos, atributos, etc., sean lo más natural posible. De manera que, si lo que maneja la clase
son los atributos de un perro, la clase deberia llamarse "Perro".

# Representación de una clase en codigo y en forma grafica.

Solamente agregamos 2 atributos o caracteristicas de la clase persona que seran nombre y apellido, aun no se estan agregando los valores, unicamente estamos
definiendo los atributos.

Como podemos ver, no son variables normales sino se conocen como atributos de la clase ya que estas variables son las características
de nuestra clase así que no es simplemente una variable individual sino corresponde al atributo de nuestra clase  Persona.
y ahora vamos a definir el método que despliega los valores que pudiera contener estos atributos.


Ahora definimos el método de la clase donde lo usarán los objetos de esta clase. en este caso vamos a definir un método público posteriormente indicamos que es de tipo void

que no va a regresar ningún tipo de información y el método se va a llamar desplegarNombre, abrimos y cerramos paréntesis y no vamos a recibir ningún

tipo de información dentro de este método. Ahora abrimos llaves y cerramos llaves y este es el cuerpo de nuestro

método.


Así que el contenido de este método simplemente va a mandar a imprimir el valor de nuestros atributos

nombre y apellido. así que hasta el momento únicamente hemos

definido la plantilla de nuestra clase.





![codigopersona](/imagenesjava/codigopersona.png "codigopersona")





![representacionpersona](/imagenesjava/representacionpersona.png "representacionpersona")


Todavía no podemos ejecutar esta clase ya que para ello necesitaríamos crear objetos y necesitamos crear
también un método main para poder ejecutar este código así que lo que hemos hecho hasta el momento es
definir simplemente nuestra plantilla o clase  llamada **Persona** la contiene dos atributos que son 
el **nombre y el apellido**  y contiene un método llamado **desplegarNombre**, esto es lo que contiene nuestra plantilla o nuestra clase.

y posteriormente lo que vamos a hacer es crear objetos de esta clase para poder utilizarla y este objeto **lo vamos a crear dentro de un método main** para que se pueda ejecutar.
Por el momento no es posible ejecutarlo necesitamos crear objetos de esta plantilla para que se pueda ejecutar.
