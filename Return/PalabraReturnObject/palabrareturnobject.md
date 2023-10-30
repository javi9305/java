`````` java


public class PalabraReturnClases {

    public static void main(String[] args) {
        Suma s = creaObjetoSuma();
        System.out.println("Resultado de llamar el metodo sumar: " + s.sumar());
    }
    //Creamos el objeto de manera indirecta.

    private static Suma creaObjetoSuma() {
        Suma suma = new Suma(4, 6);
        return suma; //regresamos una referencia del objeto y esa referencia
                     //se le asigna a la variable s.
    }

} //Termina clase PalabraRetunrClases
        
  /*
    Tambien en java es posible crear varias clases dentro de una misma clase,
    sin embargo solamente una de ellas puede ser marcada de tipo public, ya
    que es la clase que se va a poder acceder de manera publicalas
    demas clases que creemos dentro de este archivo, unicamente puede
    ser accedidas dentro de este archivo es decir dentro de estas
    clases que se definan en este archivo, no puede ser accedidas desde otras
    clases fuera de este archivo.
    */
//Se define fuera de la otra clase
class Suma {

    int a;
    int b;

    public Suma(int a, int b) {
        this.a = a;
        this.b = b;

    }
   public int sumar(){
    return this.a + this.b;
   
   }
}








`````` 

Explicacion del codigo

![returnobjeto](/imagenesjava/returnobjeto.png "returnobjeto")

Entramos al método crearObjetoSuma y la variable suma ya esta apuntando a la referencia en memoria con terminación 0x797, lo que estamos haciendo es que de la clase suma que hemos declarado, tiene 2 atributos a y b y el método sumar, entonces de esta clase estamos creando un nuevo objeto (new Suma(4,6)), se crea un nuevo objeto y se le asigno la referencia de manera dinámica el valor de 0 x 797 y entonces la variable  que está apuntando a este objeto es una variable local llamada suma que también es de tipo suma, así que la variable suma contiene la referencia 0x797, entonces al llegar a return suma, lo que se va  a regresar realmente es 0x797, de esta manera al hacer el regreso y asignarlo a la variable s, es la variable s la que va a estar apuntando al objeto con terminación 0x797, así que la variable s va a contener  0x797 y de esta manera es que va a poder acceder a los valores de a y b, con los valores que se le asignaron 4 y 6 respectivamente, por lo tanto cuando s manda a llamar el método sumar, lo que va a hacer es utilizar los atributos de la clase 4 y 6 y la llamada de sumar estos 2 valores nos va a regresar el valor de 10.