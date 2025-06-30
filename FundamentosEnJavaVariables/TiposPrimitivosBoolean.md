`````` java

public static void main (String [] args){


/*
el tipo boolean no tiene definido cuantos bits ocupa ya que esto depende de la plataforma
como del sistema operativo el cual se este trabajando, ya que un simple true o false 
que son los valores que puede soportar boolean podria ocupar 32 bits o 64 bits, esto 
depende del S.O o la plataforma.
*/



//boolean
System.out.println("True tipo boolean: " + Boolean.TRUE);
System.out.println("False tipo boolean: " + Boolean.FALSE);

/*
 se les conoce como valores de tipo bandera. una bandera basicamente 
 es como un semaforo , si esta en verde quiere decir que
 podemos continuar, si esta en rojo quiere decir que debemos detenernos.


*/
boolean booleanVar = false; 

if(booleanVar) //if(booleanVar == true) -> puede hacerse a si tambien, la otra es mas optima.
System.out.println("El valor es verdadero");

else{

System.out.println("El valor es falso");

}


var edad = 30;
/*Regresa un valor boolean y como regresa un valor boolean, var lo tomara como 
  un valor de tipo boolean. -> como si fuese asi: boolean esAdulto = edad>=18*/
var esAdulto = edad >= 18; //

System.out.println("esAdulto =" + esAdulto);



//con if
var edad = 10;
//var esAdulto = edad >= 18 -> esta linea no es tan necesaria porque puede ir dentro del if
if(edad>=18)
{
    System.out.println("Eres mayor de edad");
}
else {
    System.out.println("Eres menor de edad");
     
}
}

``````