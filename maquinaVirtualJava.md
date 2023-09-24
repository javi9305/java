![jvm](/imagenesjava/jvm.png "jvm")

Empezando con temas un poco más técnicos, podemos ver que para crear programas en Java

necesitamos agregar código a un archivo de texto y con extensión .java.

Este archivo se compila por medio del comando javac, el cual genera el código conocido como

bytecode. Este archivo generado tiene la extensión .class y es el que podemos utilizar para ejecutar nuestro programa.

Una gran ventaja de contar ya con este archivo es que sin importar dónde escribimos esta clase (por ejemplo en Windows, Mac o Linux), este archivo se puede ejecutar en cualquier ambiente, sólo

contando con una máquina virtual de Java. De esta manera podemos tener un archivo .class y

ejecutarlo en ambientes Windows, mac o Linux, o cualquier otro sistema operativo o ambiente que tenga instalada una máquina virtual. A esto se le conoce como write once / run 

anywhere, ya que a diferencia de otros lenguajes, en Java escribimos solamente una vez nuestro programa y lo podemos ejecutar en cualquier plataforma.

Esta es una de las características por las cuales Java es al día de hoy una de las tecnologías más

utilizadas a nivel mundial.

![manejo](/imagenesjava/manejomemoria.png "manejo")

Una de las cuestiones que Java simplificó muchísimo respecta al tema de manejo de memoria, fue la introducción del concepto de recolector de basura o garbage collector. A diferencia de lenguajes

como C o C++, en los cuales teníamos que manejar el concepto de apuntadores y tener bastante cuidado respecto a la localidad de memoria en donde hacia referencia los datos de nuestros

programas, en Java la asignación de datos y objetos en la memoria ram se maneja de manera

automática. Esto facilita enormemente el trabajo del programador, ya que se enfoca en tareas más importantes y productivas que el manejo de memoria.

Como programadores Java, únicamente debemos preocuparnos por crear nuestras variables, sin importar si son objetos o tipos primitivos (que veremos más adelante) y Java se encargará de

reservar el espacio de memoria necesario para la información del programa. Una vez que nuestro programa ha dejado de utilizar este espacio de memoria, el recolector de basura o 

garbage collector, detecta estos espacios de memoria y los limpia con el objetivo de reutilizarlos para que otro

programa pueda utilizar estos mismos espacios de memoria, haciendo más eficiente el uso de la misma.

Existen distintas clasificaciones respecto al manejo de memoria en Java, sin embargo esto lo

estaremos estudiando posteriormente a más detalle. De momento solo debemos quedarnos con el concepto de que es una de las simplificaciones más importantes que aportó Java respecto al 

manejo de la memoria de manera dinámica.

![ambiente](/imagenesjava/ambiente.png "ambiente")

Vamos a hablar un poco más del ambiente de ejecución de Java. En Java tenemos dos momentos importantes al momento de crear y ejecutar nuestro programa. Por un lado tenemos que 
compilar nuestro programa, pudiendo encontrar varios errores y debemos corregirlos para que nuestro

programa pueda ser compilado. Durante este proceso se dice que estamos en tiempo de

compilación, y para ello se ejecuta el comando javac (java compiler). Esto en un IDE como Netbeans, el cual utilizaremos al lo largo del curso, prácticamente con sólo ir escribiendo nuestro código o

guardar nuestro archivo estamos compilando nuestro programa, así que será muy transparente este proceso de ejecución del comando javac para nosotros. Sin embargo, haremos una 

práctica para que puedan visualizar cómo compilar cualquier programa Java desde la línea de comandos.

Por otro lado, una vez que ya se ha compilado nuestro programa y queremos ejecutarlo, se dice que estamos en tiempo de ejecución, y en este proceso de suceden varias cosas.

Por un lado Java detecta cual es la clase que se desea ejecutar, ya debe existir un archivo con

extensión .class el cual contiene los bytecodes que entiende la máquina virtual de Java. Una vez que se tiene este archivo .class se carga en memoria, y se revisa que todo esté en 

orden con el verificador de bytecode. Posteriormente se ejecuta el interprete de Java el cual hace el proceso transparente para nosotros de ejecutar nuestro archivo .class en 

cualquier plataforma, ya sea Windows, Mac,

Linux o cualquier sistema operativo o plataforma que cuente con una máquina virtual. Finalmente la máquina virtual es la que permite ejecutar nuestro programa sobre el hardware y 

sistema operativo seleccionado.

Este es el proceso general cuando creamos, compilamos y ejecutamos nuestros programas en Java.