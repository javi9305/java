### Clase PruebaAritmetica

``````java

public static void main(String[] args){
  /*
   Variables locales
   Si definimos variables locales (y son locales debido a que estamos dentro de un metodo), si estamos dentro de un metodo entonces cualquier variable que
   definamos,es una variable local, ya sea los argumentos que estamos recibiendo,asi como las variables que definamos dentro de los metodos. Por ejemplo:

    void suma(int a, int b) <- Recibiendo argumentos (son variables locales).
  
  */

  int operandoA = 6;
  int operandoB = 2;

}
//Este metodo solo es para verificar que operandoA, no se puede usar en otro metodo.
public void otroMetodo(){
 
  System.out.println(operandoA); // <- marca error.Esto no es posible, nos indica que el simbolo no se reconoce. ¿por que sucede este error? 

  /*
   Esto se debe a que la variable operandoA solo va a estar disponible dentro del bloque de codigo en el cual fue definida. Y como esté ya es otro bloque de codigo (nos referimos al metodo otroMetodo), entonces la variable operandoA no puede ser accedida desde otro bloque de codigo. Por lo tanto no nos reconoce la variable operandoA.
 
   Si definimos una variable a nivel de la clase, entonces la variable que definamos fuera de los metodos se va a poder acceder durante toda la clase.

  
  */

}


//Creamos un objeto de la clase Aritmetica enviando argumentos
       //Usamos las variables locales para inicializar nuestro objeto aritmetica.

       /*
        Estamos utilizando nuestras variables locales para inicializar nuestro objeto aritmetica,
        posteriormente nuestro objeto aritmetica con los valores de las variables locales recibidas
        inicializa los atributos de la clase.
       */
       Aritmetica objeto1 = new Aritmetica(operandoA,operandoB); //Se pasan los argumentos al constructor de la clase Aritmetica.
       
       //Imprimimos los valores de los operandos
       /*
        Tambien podemos observar que podemos imprimir  y acceder a las variables locales, si estamos dentro
        del mismo metodo donde se han definido estas variables(operandoA y operandoB).
       */
        System.out.println("operandoA = " + operandoA);
        System.out.println("operandoB= " + operandoB);
        




        /*  
        ya que hemos inicializado los atributos del objeto aritmetica, entonces podemos a mandar 
        a llamar los metodos sumar,restar, etc.
        */

        //Imprimimos el resultado de la suma
        System.out.println("\nResultado suma:" + objeto1.sumar());
        
        //Imprimimos el resultado de la resta
        System.out.println("\nResultado resta:" + objeto1.restar());
       
        //Imprimimos el resultado de la multiplicacion
        System.out.println("\nResultado suma:" + objeto1.multiplicar());
        
        //Imprimimos el resultado de la division
        System.out.println("\nResultado suma:" + objeto1.dividir());
    }



``````


### Clase Aritmetica

`````` java

public class Aritmetica {
    /*
    Atributos de una clase.
    Cuando creamos un objeto, los atributos de la clase se asocian al objeto y unicamente los atributos de la clase se van a destruir
    hasta el momento que se quite el objeto de la memoria, asi que los atributos de la clase lo podemos utilizar en los diferentes metodos y durante todo el tiempo que el objeto de la clase que se ha creado este disponible en la memoria.


    los atributos a y b, se estan definiendo fuera de cualquier metodo, incluyendo los constructores, por lo tanto estas variables se pueden acceder en toda la clase, pero recordemos que para poder acceder a los atributos a y b, debemos crear un objeto, asi que realmente lo que vamos a poder acceder son estas variables a y b, una vez se haya creado el objeto y lass vamos a poder acceder durante todo el tiempo de vida que el objeto este disponible en memoria y el único que puede quitar el objeto de la memoria es el recolector de basura, una vez que no tenemos ninguna variable apuntando al objeto.

    Nosotros no vamos a controlar en que momento se quita un objeto de la memoria, por lo tanto vamos a poder acceder a los atributos durante todo el tiempo de un objeto de la clase Aritmetica este disponible en memoria.
    
    */
    int a;
    int b;
    
     //Constructor
    public Aritmetica() {
        System.out.println("Ejecutando constructor vacio");
    }
    //Recibe los 2 argumentos: operandoA y operandoB
    public Aritmetica(int arg1, int arg2){
        a = arg1;
        b = arg2;
        System.out.println("Ejecutando constructor con dos argumentos");
    
    }
    
    
    /*
    
     Una vez que definimos atributos de nuestra clase, podemos accederlo a lo largo de nuestra clase, en cada uno de los metodos que utilizamos.
    
    */
    // Metodo sumar que retorna una suma.
    public int sumar() {
        return a + b;
    }
    
    public int restar(){
        return a - b;
    } 
    public int multiplicar(){
        return a * b;
    }
    
    public int dividir(){
     return a/b;
    }
}

``````


