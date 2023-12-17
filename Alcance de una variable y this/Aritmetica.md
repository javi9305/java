
`````` java

public class Aritmetica {
    
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