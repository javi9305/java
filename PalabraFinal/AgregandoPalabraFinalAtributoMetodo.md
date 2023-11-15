![clasefinal2](/imagenesjava/clasefinal2.png "clasefinal2")


explicación de codigo cuando un objeto tiene la palabra final



Al momento de definir una variable de tipo Object como en este caso VAR_PERSONA, LA MARCAMOS COMO FINAL ENTONCES LE tenemos que asignar la referencia de un objeto y ya no podrá apuntar a otro objeto, siempre va a apuntar al mismo objeto, pero el estado del objeto si lo puede modificar , asi que la primera vez manda a llamar el método setNombre de este objeto y cambio el valor de nombre(por default era null) a juan y para recuperar este valor manda a llamar el método getNombre, y la siguiente vez lo que hizo fue como está apuntando al mismo objeto entonces cambia el valor de juan a Carlos y se aplica el mismo procedimiento de set y get.


![clasefinal3](/imagenesjava/clasefinal3.png "clasefinal3")





`````` java

public class ClaseFinal {
  //Variables marcadas como final
    /*Esta variable como no se ha definido como static,
      esta variable no la podremos acceder con el nombre de nuestra clase punto
      el nombre de la variable.
    */
    public final int varNumero = 10; //No se puede modificar posteriormente.
    
    //Constante en java
    public static final int VAR_PRIMITIVO = 15;
    
    /*
    una vez que le asignamos esta referencia, esta variable persona ya no
    va a poder apuntar a otro objeto, sin embargo si puede modificar el
    estado del objeto es decir sus atributos.
    */
    public static final Persona VAR_PERSONA= new Persona();
    
    //Metodo final.
    public final void metodoFinal(){
    
    
    }
    
    class ClaseHija extends ClaseFinal{
       /*
        Con la palabra final en un metodo, ya no vamos a poder sobreescribir 
        el comportamiento definido en la clase padre es decir el metodoFinal
        */
            
        //No es posible modificar el comportamiento(sobreescritura)
        //de un metodo padre marcado como final
        
        
        //public void metodoFinal(){ -> marca error.
        //}
    }
    
    
}


``````