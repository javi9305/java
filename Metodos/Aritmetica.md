
`````` java

public class Aritmetica {
    
    /*No se puede utilizar var en la definicion del metodo
        por ejemplo: public var sumar (int a, int b)
    
    esto debido a que var no indica el tipo que queremos regresar, por lo tanto
    se debe especificar el tipo que se quiere regresar,
    
    tampoco se puede utilizar var para la defincion de los argumentos de nuestro metodo
    ya que de igual manera no sabriamos de que tipo es el argumento que queremos recibir.

    */
    public int sumar(int a, int b){  //recibe 2 valores

        /*
        realiza la suma y finalmente este resultado se regresa a la clase que va a hacer la llamada a este metodo.
        y debe corresponder con el tipo de dato que se indico que va a regresar este metodo. por ello el resultado debe ser de tipo entero, ya que se indico que el valor que se va a regresar es de tipo entero  
        
        */
        return a + b; //              
        
    
    }
    
}

`````` 