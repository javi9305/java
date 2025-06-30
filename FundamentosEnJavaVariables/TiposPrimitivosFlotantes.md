
`````` java

public static void main (String [] args){

float floatVar = 1000
//1000.0 se imprime este valor es decir que en automatico se agrega un decimal.
System.out.println("floatVar = " + floatVar); 


/*
si a nuestro numero le agregamos un tipo flotante, marcaria un error ya que por 
default las literales en java de tipo flotante  son de tipo double.

El error que marca es incompatibilidad de tipos, ya que existe posible perdida de 
informacion al querer convertir la literal de tipo double a tipo float.

*/
float floatVar = 1000.10 
                         
System.out.println("floatVar = " + floatVar); 


//para eso debemos especificar que esta literal 1000.10 es de tipo float utilizando la letra F asi: 1000.10F

float floatVar = 1000.10F; // los ceros hacia la derecha se omiten.
System.out.println("floatVar = " + floatVar); //Imprimiria 1000.1


//Informacion de tipo float

System.out.println("bits tipo float:  = " + float.SIZE);
System.out.println("floatVar = " + float.BYTES);
System.out.println("floatVar = " + float.MIN_VALUE);
System.out.println("floatVar = " + float.MAX_vALUE);

//Tambien podemos especificar valores de tipo double.

double doubleVar = 100D
System.out.println("doubleVar = " + doubleVar);

System.out.println("bits tipo double:  = " + Double.SIZE);
System.out.println("doubleVar = " + Double.BYTES);
System.out.println("doubleVar = " + Double.MIN_VALUE);
System.out.println("doubleVar = " + Double.MAX_vALUE);

}


`````` 