
`````` java

public class Aritmetica {
    
    //Constructor
    public Aritmetica(){
        System.out.println("Ejecutando constructor vacio");
    
    }
    
    
    
    //Metodo sumar que recibe 2 argumentos y regresa el resultado.
    /*los argumentos de un metodo pasan a hacer variables locales donde se puede utilizar
    dentro de este metodo*/
    public int sumar(int a, int b) {

        return a + b;

    }
    
    //Metodo resta que recibe 2 argumentos y regresa el resultado.
    public int restar(int a, int b){
    
       return a - b;
    }
    //Metodo multiplicacion que recibe 2 argumentos y regresa el resultado.
    public int multiplicar(int a, int b){
       
       return a * b;
    }
    
    //Metodo division que recibe 2 argumentos y regresa el resultado.
    public double dividir(int a, int b){
    
        return a / b;
    }
    
}

``````