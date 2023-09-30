
# Tipos primitivos

`````` java

public static void main (String [] args){

//byte, short, int, long


//Si asignamos el valor de 128  marcara el error de posible perdida de conversion al querer asignar un tipo entero que es la literal 128 a un tipo byte.
//si la literal cumple con el minimo y el maximo entonces es posible asignarlo al tipo byte
//Por default las literales en java son de tipo entero.

byte byteVar = 127;
//Extraemos la información de tipo byte

System.out.println("byteVar = "+ byteVar);
System.out.println("bits tipo byte " + Byte.SIZE);
System.out.println("bytes tipo byte " + Byte.BYTES);
System.out.println("valor minimo tipo byte " + Byte.MIN_VALUE);
System.out.println("valor maximo byte " + Byte.MAX_VALUE);


short shortVar = 32767;
//Extraemos la información de tipo short

System.out.println("shortVar = "+ shortVar);
System.out.println("bits tipo short " + Byte.SIZE);
System.out.println("bytes tipo short " + Byte.BYTES);
System.out.println("valor minimo tipo short " + Short.MIN_VALUE);
System.out.println("valor maximo short " + Short.MAX_VALUE);



int intVar = 2147483648; // (el maximo del int es 2147483647 )nos marcaria error de compatibilidad , ya no nos marca posible perdida de información sino que nos indica que el tipo entero es demasiado largo.
//Extraemos la información de tipo int

System.out.println("intVar = "+ intVar);
System.out.println("bits tipo int " + Integer.SIZE);
System.out.println("bytes tipo int " + Integer.BYTES);
System.out.println("valor minimo tipo int" + Integer.MIN_VALUE);
System.out.println("valor maximo tipo int " + Integer.MAX_VALUE);



//Este valor en el ide estaria marcando un error porque es un numero demasiado grande.
long longVar = 9223372036854775807; //recordemos que si no establecemos otra cosa esta literal es de tipo entero es decir que su valor maximo es 2147483647 y se esta escribiendo un numero mas grande, el error que arroja es: el valor del entero es demasiado largo. ¿Como hacemos para utilizar este tipo long?  necesitamos indicar que esta literal debe de ser de tipo long y para hacerlo en java solo ocupariamos una L por ejemplo quedaria asi: 9223372036854775807L, entonces esta literal se convierte en automatico en una literal de tipo long. una cosa es el tipo de la variable  y otra cosa es el tipo de la literal. debemos tener cuidado con ambas cuestiones cuando estamos trabajando con java ,ya que no solamente es el tipo de dato sino tambien el valor de la literal que estamos utilizando, debemos estar seguros que el valor de la literal corresponda con el valor que necesitamos.

//Extraemos la información de tipo long

System.out.println("longVar = "+ longVar);
System.out.println("bits tipo long " + Long.SIZE);
System.out.println("bytes tipo long " + Long.BYTES);
System.out.println("valor minimo tipo long" + Long.MIN_VALUE);
System.out.println("valor maximo tipo long" + Long.MAX_VALUE);


//Manejos de tipo utilizando la variable var

var numero = 127; //seria de tipo byte por que soporta el valor sin ningun problema.

//si nos pasamos del valor maximo del byte entonces podemos  asignar el valor de 128, esto quiere decir que esta variable no es de tipo byte  ya que soporta un valor mayor a su valor maximo.

var numero = 128;

//ponemos el valor de tipo short (32767) y lo aumentamos en 1.

var numero = 32768 //como lo podemos asignar entonces esta variable no es de tipo short, ya que pudimos superar el valor maximo de tipo short.

//vamos asignar el valor maximo del tipo int.
var numero = 2147483647; // el valor maximo de tipo int lo podemos asignar sin ningun problema

var numero = 2147483648 // pero si pasamos el valor maximo, entonces quiere decir que esta variable es de tipo long ya que no pudimos superar el valor maximo del tipo entero. por lo tanto quiere decir que esta variable por default si le asignamos un valor de tipo numero , por default va a ser de tipo entero, sin embargo tambien la podriamos convertir a tipo long simplemente conviertiendo la literal a un tipo long (2147483648L) y por lo tanto detecta que necesitamos del lado izquierdo una variable que soporte esta literal  de tipo long, y nuestra variable en este momento se convierte  de tipo entero a un tipo long, ya que asi lo hemos establecido , necesitamos una variable tal que soporte un valor de tipo long. dependiendo de tipo que necesitemos declaramos la literal  y en automatico var va a definir el tipo que necesitamos para nuestra literal.


}

`````` 