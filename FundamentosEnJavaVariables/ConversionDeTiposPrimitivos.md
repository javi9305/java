
`````` java
public static void main (String [] args){

//Convertir un String a un tipo int

/*
recibe un string. lo que hara esta linea va a convertir el string a entero, el 
resultado de esta expresion, de llamar esta funcion (parseInt) es el valor de 20 
pero ya en entero es decir regresa el valor 20.
*/
var edad = Integer.parseInt("20"); 


//Convertir de String a un tipo double
var edad = Double.parseDouble("3.1416");

/*No tenemos conversion de cadena a tipo char , ya que un String tiene 1 o mas caracteres 
  y un char solo puede almacenar un solo caracter pero lo que puede hacer es lo siguiente:
*/
char c = "Hola".charAt(0); //tomaremos uno de los caracteres de la palabra Hola.
//        0123 = 4 elementos//chartAt: un caracter en cierta posicion del String
         //las posiciones del 0 al 3


/*
la clase scanner utiliza el metodo nextLine para leer informacion de la consola sin embargo
esto nos regresa un tipo String, y por lo tanto si lo queremos asignar a un tipo entero no 
vamos a poder realizar la asignacion directamente. 
*/


var scanner = new Scanner(System.in);
/*el metodo parseInt recibe como valor lo que escribamos en la consola. y 
  posteriormente realiza la conversion a tipo entero.*/
int edad = Integer.parseInt( scanner.nextLine() ); 


//escribe una cadena y solo tomara la primera letra es decir que se encuentre en la posicion 0.
char caracter = scanner.nextLine().charAt(0); 



//Convertir de int a String

//con esta funcion convertimos el tipo entero a un string y solo se podra imprimir  y unir con otra cadena.
String edadTexto = String.valueOf(25); 


//Conversion entre tipos.

short s = 10;
/*
esta asignacion no la podemos realizar directamente, ya que un tipo byte solo tiene 8 bits para almacenar
la informacion en cambio un short tiene 16 bits por lo tanto, un tipo short no cabe directamente en un tipo byte.
*/
byte b = s; 

//si la variable b fuera de tipo entero
short s = 10;
/*si se puede asignar, ya que un tipo short ocupa 16 bits y el tipo entero ocupa 32 bits, 
  un tipo entero sin problemas puede almacenar un tipo short.*/
int b = s; 



/*
Debido a que el valor 10 es valido tanto para un tipo short como para un tipo byte, para hacer 
esta asignacion podemos hacer lo que se conoce como casting o conversion entre tipos.
*/


short s = 10;
byte b = (byte) s; //conversion. regresara el valor de 10 de tipo byte 



/*Debemos tener cuidado cuando hagamos esta conversion ya que esto byte b = (byte) s puede 
provocar perdida de informacion  ya que un tipo short tiene 16 bits y un tipo byte tiene 8 bits, 
asi que si asignamos un valor que no soporta el tipo byte como por ejemplo 129. el short lo podra
almacenar sin ningun problema ya que su valor maximo del short es 32625 aprox. pero el byte su valor
maximo es 127. Al compilador indicarle que queremos hacer una conversion de manera obligatoria, 
entonces el valor de 128 lo va a asignar a byte b sin ningun problema, pero debido a que 128 no 
cabe en un byte, va a ver perdida de informacion por lo tanto si se manda a imprimir el valor de 
la conversion dara esto: -128.

pero como le indicamos al compilador que estamos seguros de la conversion, 
ya es problema nuestro el hacer la conversion.
ya que por default el compilador nos indica que los tipos son incompatibles, 
el tipo short no se puede asignar al tipo byte ya que puede existir perdida de informacion.

*/
}






`````` 