`````` java

public static void main (String [] args){



//el tipo boolean no tiene definido cuantos bits ocupa ya que esto depende de la plataforma como del sistema operativo el cual se este trabajando,
// ya que un simple true o false  que son los valores que puede soportar boolean podria ocupar 32 bits o 64 bits, esto depende del S.O o la plataforma.


//boolean
System.out.println("True tipo boolean: " + Boolean.TRUE);
System.out.println("False tipo boolean: " + Boolean.FALSE);

boolean booleanVar = false;

if(booleanVar) //if(booleanVar == true) -> puede hacerse a si tambien, la otra es mas optima.
System.out.println("El valor es verdadero");

else{

System.out.println("El valor es falso");

}


var edad = 30;
var esAdulto = edad >= 18; //Regresa un valor boolean y como regresa un valor boolean, var lo tomara como un valor de tipo boolean. -> como si fuese asi: boolean esAdulto = edad>=18

System.out.println("esAdulto =" + esAdulto);


}

``````