

`````` java

public class PalabraThis {
    public static void main(String[] args) {
      Persona persona = new Persona("Juan");  
    }
}


class Persona{
  String nombre;
  
  Persona(String nombre){
    this.nombre = nombre; //apunta a un objeto de tipo Persona
      System.out.println("impresion del operador this dentro de la clase Persona: " + this);//this apunta a un objeto de tipo Persona en este momento.
    Imprimir imprimir = new Imprimir();
    imprimir.imprimir(this); //this contiene una referencia al objeto persona
                             //Hasta que se empieze a ejecutar el metodo imprimir es que va a cambiar el operador this.
  
  }


}
/*el operador this funciona unicamente en el momento que se esta ejecutando cierto objeto*/
class Imprimir{
   public void imprimir(Persona p){
       System.out.println("impresion argumento persona: " + p); //valor del objeto persona.
       System.out.println("Impresion objeto actual (this )" + this); // this apunta a un objeto de tipo imprimir en este momento.
   
   }
}

``````


Explicacion del codigo.

Estamos dentro del constructor Persona y como podemos ver tenemos la variable this.

![palabrathis1](/imagenesjava/palabrathis1.png "palabrathis1")

Ahora estamos dentro de la clase Imprimir, pero como no creamos ningún constructor, en automático el compilador java crea uno sin que nosotros lo veamos.
Hasta que se empiece a ejecutar el método imprimir es que va a cambiar el operador this. 

![palabrathis2](/imagenesjava/palabrathis2.png "palabrathis2")

 
El apuntador this, apunta a diferente objeto dependiendo cual sea la clase que se esté ejecutando.
La única restricción de la palabra this es que no debe estar dentro de un método estático.
El contexto estático esta relacionado con una clase y el operador this este asociado con objetos.
