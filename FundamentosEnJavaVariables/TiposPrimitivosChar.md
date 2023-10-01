
`````` java

public static void main (String [] args){







System.out.println("bits tipo char:  = " + Character.SIZE);
System.out.println("doubleVar = " + Character.BYTES);

//Estos valores minimos y maximos corresponden a la tabla unicode. Pero el juego de caracteres unicode puede varia de sistema operativo en sistema operativo.
System.out.println("doubleVar = " + Character.MIN_VALUE); //el valor minimo es null, el valor minimo puede varias dependiendo de la plataforma en la cual estemos trabajando.
System.out.println("doubleVar = " + Character.MAX_vALUE); //el valor maximo es signo de ?

// un tipo char soporta un caracter, para ello se utiliza comilla simple.
char varChar = 'a';
System.out.println("varChar = " + varChar);

//Podemos utilizar tanto el valor unicode o en decimal para imprimir el valor de un caracter.
// /u para indicar a java que es un unicode

char varChar = 'u/0021';
System.out.println("varChar = " + varChar); // se imprime el caracter del signo de exclamacion !

//En decimal
char varCharDecimal = '33'; //Debido a que utilizamos un tipo char en automatico entiende que debe convertir el numero entero a un tipo char
System.out.println("varCharDecimal = " + varCharDecimal); // se imprime el caracter del signo de exclamacion !

//se puede tambien hacer con el simbolo !
char varCharSimbolo = '!'; 
System.out.println("varCharSimbolo = " + varCharSimbolo);



//Cuando usamos var

var varChar = 'u/0021';  //si usamos el codigo unicode, en automatico al encontrar el simbolo del caracter unicode, tambien el lado izquierdo se convierte en una variable de tipo char.
System.out.println("varChar = " + varChar); 

//en el caso del decimal
char varCharDecimal = '33'; //ya no indicamos en ningun momento que este valor es de tipo unicode por el contrario en caso de definir una variable de tipo char, va a definir una variable de tipo numerico.
System.out.println("varChar = " + varCharDecimal);






}