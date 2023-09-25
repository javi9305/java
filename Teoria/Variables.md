# ¿Que es lo que necesitamos si queremos almacenar información?


Necesitaremos crear variables que nos permita almacenar información.


# ¿Que es una variable?



Es un espacio de memoria que nos ayuda a almacenar un valor y va a tener un **identificador**. Sin embargo este valor puede **cambiar o modificarse** a través del tiempo.



# ¿Las variables almacenan la información de un programa permanentemente?




No. lo hacen de **manera temporal**.
Los datos que tengamos **pueden ir cambiando a lo largo de la ejecución** del programa es decir **esta información va a variar según lo que estemos recibiendo por parte del usuario o del tipo de información que estemos procesando.**




# ¿Cuales son los objetivos de crear o declarar variables?



* Reservar espacio de memoria dependiendo el **tipo de dato** que se utilice.

* Almacenar nuestros **Datos o Valores** durante **la ejecución del programa**.


# ¿Por qué las variables estan relacionadas con la memoria RAM?


* Ocupan un **espacio** en memoria RAM
* Poseen un nombre simbólico o **identificador**
* El espacio ocupado **tiene un valor especifico o valor de la variable**
* El valor de una variable **puede o no cambiar muchas veces**


# ¿Cuáles son los tipos de datos que puede almacenar una variable?


* Números
* Cadenas
* Referencias a objetos

# ¿Cuáles son los 3 pasos que necesitamos para crear una variable?

* Primero tenemos que especificar el tipo en java que vamos a utilizar.
* Posteriormente un identificador o nombre de la variable.
* Se le asigna un valor dependiendo el tipo especificado.


# ¿Cómo es la declaración de una variable?

`Int` **(el tipo de dato)**     `NombreDeLaVariable` **(Identificador)** = `15` **(Valor)** dentro del cuerpo del programa.

# ¿Como funciona de manera interna esta declaración de variable?

Lo que hara la memoria RAM es internamente **apartar 4 bytes en memoria y crear una variable de tipo int que va a ocupar 4 bytes.**
Entonces esos 4 bytes van a pertenecer a la variable **NombreDeLaVariable**, la cual se va a identificar como la variable **NombreDeLaVariable**.
Teniendo reservado los 4 bytes de espacio en la memoria **se le asignara el valor 15** y en caso de que no tuviera nada solamente estaria reservado ese
espacio de memoria.


# ¿Como se representa de manera grafica?

`Int numero = 15`

![Variable](/imagenesjava/VariableJava.jpg "FOTO")


# ¿Cómo imprimimos el valor de la variable declarada?
En caso de querer mostrar el **valor 15 en pantalla se imprimará la variable a.**
 Para imprimir esa variable en pantalla utilizamos el método **System.out.println (a)** el cual lleva dentro la variable a **donde su función es pedirle que imprima esa variable** y entonces va a buscar a la memoria RAM, el sector con la porción de memoria que está identificada como a  y cuando la encuentre entra  dentro del espacio asignado y checa cual es el valor que **tiene almacenado el cual es 15.**

# ¿Cuáles son las reglas para declarar una variable?

**Regla #1**

* No tener el mismo nombre que una “palabra reservada”	Ejemplos: static, class, public, private, doublé, int, float, byte, true, false.     
    * Palabras mal reservadas: int class o byte default.

**Regla #2**

 * Un nombre de variable solo pueden ser letras, dígitos y el guion bajo o subguion.
    * Variable bien declarada: int programando19 o float numero_float
    * Variable mal declarada: Int %programando o float variable-numérica.


**Regla #3**

* Una palabra debe comenzar con un carácter(letra)o con un guion bajo no podemos utilizar números como primer carácter .
    * Variable bien declarada: Int programando19 o int_programando.
    * Variable mal declarada: Int 19programando.

**Regla #4**

 * No pueden tener espacio en blanco.
	  * Variable bien declarada: Int variable_numerica  o float variable.
    * Variable mal declarada: Int variable numérica.


# ¿Una variable que fue definida dentro de un método por ejemplo el método main puede ser utilizada fuera de este método main?

No. A esto se le conoce como alcance de una variable.


# ¿Podemos reutilizar las variables?

Si. Pero tiene restricciones.


# ¿Qué restricción tiene una variable?

No las podemos acceder en cualquier parte de nuestro programa sino dependiendo donde se haiga definido esta variable  va a ser en los lugares donde podemos utilizar la variable.


# ¿Es necesario volver a especificar el tipo de dato cuando usamos la variable?

No. Una vez que se declara la variable no es necesario volver a especificar el tipo de dato ya que definir otra vez la variable marcaria error.

# ¿Como se conoce el valor que le asignamos a una variable?

Literal

# ¿Solo las variables tienen un tipo de dato?
No. Las literales también tendrán un tipo. Por ejemplo el numero 10 es de tipo int.

# ¿Qué nombre se le da a la información que le asignamos a nuestras variables?

Información en código duro






# Notación de camello


# ¿Qué es la notación de camello?

Se refiere a que si escribes una palabra debe escribirse respetando esta notación, por ejemplo la palabra:
          
  **variablePersona**

Observa que son dos palabras, entonces **la primera letra de cada palabra es la que debes poner atención**. **Si es una variable la primera letra va en minúsculas** pero después cada **primera letra de cada palabra va en mayúscula**(solo la primera letra).

Otro ejemplo            

      unaVariableMasLarga

**Se le llama de camello por qué si observas hace una curva cada que pones una letra en mayúscula**.
Esto se usa para que sea fácil leer las variables, ya que si pones:

      unavariablemaslarga

Todo en minúscula puedes observar que es muy difícil leer la variable y no es posible distinguir cuando inicia una palabra y cuando termina otra palabra.


# ¿Si tenemos más de una palabra para el identificador de la variable que  se recomienda  hacer?
                
 Se recomienda **usar letra mayúscula en la segunda palabra** a esto se le conoce como notación de camello ejemplo:

      miVariableEntera



# ¿Con que otro nombre se le conoce a la notación de camello?
Altas y bajas 


# Palabra reservada var

# ¿Qué es var?

var es para no tener qué especificar el tipo de dato de manera formal, sino que es inferido según el tipo de dato de la literal que le asignas.

Por ejemplo:
`var miVariable = 1;`

debido a que la literal 1 es de tipo int entonces **tu variable infiere que debe ser de tipo int**, es todo, no te ayuda en otra cosa, sólo en inferir tipos.

# ¿Cuál es el objetivo de la palabra var?

Es para simplificar la declaración de las variables y para hacer más legible el código es decir en lugar de leer una declaración de una variable con un tipo de datos muy extenso, solo usas var y listo.

# ¿A partir de que versión de java podemos usar la palabra var?

a partir de la versión 10 de java ya que podemos usar la palabra reservada var.

# ¿Qué es lo que sustitute la palabra var?

 el tipo de dato definido.

# ¿Cómo funciona la palabra reservada var? 

Se coloca simplemente var en vez del tipo de dato definido para que java infiera el tipo de dato que estamos utilizando.

# ¿Cómo va a inferir el tipo de dato? 

el tipo de dato lo va a inferir a partir de la literal que estamos utilizando.
Por ejemplo:

`Int miVariable = 10;`

`Var miVariable = 10;`

# La importancia de las variables
`````` java

// sin usar una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        
   //Imprimira 3 veces la palabra saludos!!     
   System.out.println("Saludos!!!")
   System.out.println("Saludos!!!")
   System.out.println("Saludos!!!")

   //si se quisiera hacer una modificación se tendria que hacer en cada linea.
   //esto no es lo mas práctico si queremos realizar cambios de una sola vez.
   System.out.println("Saludos");
   System.out.println("Saludos");
   System.out.println("Saludos");

    }

``````


`````` java

// Usando una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        //Agregar la cadena de saludos en una variable
           String saludar = "saludos";

 //en lugar de usar la cadena vamos a utilizar la variable y se imprimira lo que contiene la variable saludar
   System.out.println(saludar);
   System.out.println(saludar);
   System.out.println(saludar);

    }

``````

`````` java

// cambiando contenido de una variable
public class HolaMundo {
    

    public static void main(String[] args) {
        
           String saludar = "saludos desde java"; //si quisieramos hacer un cambio solo lo hariamos en un solo lugar en este caso la variable saludar.

 //este cambio se replicara en la variable saludar.
   System.out.println(saludar);
   System.out.println(saludar);
   System.out.println(saludar);

    }

``````
