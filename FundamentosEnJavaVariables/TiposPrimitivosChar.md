
`````` java

public static void main (String [] args){





//Informacion del tipo char

System.out.println("bits tipo char:  = " + Character.SIZE);
System.out.println("doubleVar = " + Character.BYTES);

/*Estos valores minimos y maximos corresponden a la tabla unicode. Pero el juego de caracteres unicode puede 
varia de sistema operativo en sistema operativo.
*/

//el valor minimo es null, el valor minimo puede varias dependiendo de la plataforma en la cual estemos trabajando.
System.out.println("doubleVar = " + Character.MIN_VALUE); 
//el valor maximo es signo de ?
System.out.println("doubleVar = " + Character.MAX_VALUE); 

// un tipo char soporta un caracter, para ello se utiliza comilla simple.
char varChar = 'a';
System.out.println("varChar = " + varChar);

//Podemos utilizar tanto el valor unicode o en decimal para imprimir el valor de un caracter.
// /u para indicar a java que es un unicode

char varChar = 'u/0021';
System.out.println("varChar = " + varChar); // se imprime el caracter del signo de exclamacion !

//En decimal

/*
Debido a que utilizamos un tipo char en automatico entiende que debe convertir 
el numero entero a un tipo char
*/
char varCharDecimal = '33'; 

// se imprime el caracter del signo de exclamacion !
System.out.println("varCharDecimal = " + varCharDecimal); 
//se puede tambien hacer con el simbolo !
char varCharSimbolo = '!'; 
System.out.println("varCharSimbolo = " + varCharSimbolo);



//Cuando usamos var

/*
si usamos el codigo unicode, en automatico al encontrar el simbolo del caracter unicode,
 tambien el lado izquierdo se convierte en una variable de tipo char.
*/
var varChar = 'u/0021';  
System.out.println("varChar = " + varChar); 

//en el caso del decimal

/*
ya no indicamos en ningun momento que este valor es de tipo
unicode por el contrario en caso de definir una variable de tipo char, 
va a definir una variable de tipo numerico.
*/
char varCharDecimal = '33'; //
System.out.println("varChar = " + varCharDecimal);


//Se puede usar el var sin ningun problema con el simbolo


var varCharSimbolo = '!'; 
System.out.println("varCharSimbolo = " + varCharSimbolo);


int variableEnteraSimbolo = '!'; //Imprimira el valor de 33.

int letra = 'a'; //Imprimira el valor de 97.




}