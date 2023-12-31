# ¿Cuales son las caracteristicas de una clase?

* Una clase es una plantilla.
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

Es una plantilla para poder crear objetos es decir podremos generar objetos (instancias) para que puedan
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
necesitamos **crear objetos a partir de esa plantilla.** Definir la clase **no crea un objeto en automático, tenemos que crearlos.**


Por ejemplo:


![ejemploclase](/imagenesjava/ejemploclase.png "ejemploclase")


# ¿Por medio de que se extrae la información del mundo real?

Atributos y métodos.

# ¿Cómo debe ser los nombres de una clase?

lo ideal es que los nombres de las clases, métodos, atributos, etc., sean lo más natural posible. De manera que, si lo que maneja la clase
son los atributos de un perro, la clase deberia llamarse "Perro".

# ¿Una clase podria llamarse usuario?

la clase puede tener cualquier nombre siempre y cuando respetes las reglas de nombres de variables en Java (numeros o letras y signos de _ al inicio si lo deseas)

Asi que una clase sin problemas puede llamarse Usuario. Recuerda que la primera letra de cada palabra en una clase debe ir en mayuscula.

# ¿Una clase siempre debe bautizarse con un nombre en singular?

Lo normal es que se bauticen en singular ya que una clase es una plantilla de la cual **generaras objetos**, entonces, cuando creas una instancia de la clase hace referencia a un solo objeto, por ello es un Usuario y no varios Usuarios. Asi que las clases es común que sean escritas en singular.

Veras otras estructuras de datos como arreglos o colecciones que hacen referencia a muchos elementos, por lo que si se llamarán en plural, como usuarios, pero eso hace referencia a la variable que almacena varios elementos, el tipo de java sigue siendo singular.


# Representación de una clase en codigo y en forma grafica.

* Solamente agregamos 2 atributos o caracteristicas llamados nombre y apellido de la **clase persona**, aun no se estan agregando los valores, unicamente estamos
definiendo los atributos.

Como podemos ver, no son variables normales sino se conocen como **atributos de la clase** ya que estas variables son las características
de nuestra clase, así que no es simplemente una variable individual sino corresponde al atributo de nuestra **clase Persona**.

* Ahora definimos el método que despliega los valores que pudiera contener estos atributos de la clase donde lo usarán los objetos. 

en este caso vamos a definir un **método público** posteriormente indicamos que es de **tipo void** que no va a regresar ningún tipo de información y el método se va a llamar **desplegarNombre**, entonces abrimos y cerramos paréntesis ya que no vamos a recibir ningún tipo de información dentro de los parentesis. Ahora abrimos llaves para escribir lo que se requiere imprimir y el contenido de este método simplemente va a mandar a imprimir el valor de nuestros atributos  **nombre y apellido**  y luego cerramos llaves y este es el cuerpo de nuestro método.

**Así que hasta el momento únicamente hemos definido la plantilla de nuestra clase.**





![codigopersona](/imagenesjava/codigopersona.png "codigopersona")




Si lo vemos de forma grafica.

![representacionpersona](/imagenesjava/representacionpersona.png "representacionpersona")


Asi como esta el dibujo todavía no podemos ejecutar esta clase ya que para ello necesitaríamos crear objetos (el circulo pequeño rojo seria el objeto) y necesitamos crear
también un método main para poder ejecutar este código así que lo que hemos hecho hasta el momento es
definir simplemente nuestra plantilla o clase  llamada **Persona** la contiene dos atributos que son 
el **nombre y el apellido**  y contiene un método llamado **desplegarNombre**, esto es lo que contiene nuestra plantilla o nuestra clase.

y posteriormente lo que vamos a hacer es crear objetos de esta clase para poder utilizarla y este objeto **lo vamos a crear dentro de un método main** para que se pueda ejecutar.
Por el momento no es posible ejecutarlo necesitamos crear objetos de esta plantilla para que se pueda ejecutar.
