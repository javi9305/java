
`````` java

public class Operaciones {
    /*
    - A JAVA UNICAMENTE LE INTERESA REVISAR LOS TIPOS DE DATOS.
    - Se verifica el ORDEN DE LOS TIPOS
      por ejemplo si tenemos un metodo sumar(int,double) o sumar(double,int)
    - Podemos modificar el tipo de retorno, no importa si los tipos son diferentes
      tambien se cosideran una sobrecarga de metodo.
    - No importa si son privados o publicos siguen siendo una sobrecarga de metodos.
    
    */
    //Metodo sumar
    public static int sumar(int a, int b){
        System.out.println("Metodo sumar(int,int)");
        return a + b;
    }
    
    //sobrecarga del metodo sumar
    public static double sumar(double a, double b){
        System.out.println("Metodo sumar(double,double)");
    return a + b;
    }
    
    public static double sumar(int a, double b){
        System.out.println("Metodo sumar(int, double)");
        return a + b;
  
    }
    
    public static double sumar(double a, int b){
        System.out.println("Metodo sumar(double,int)");
        return a + b;
    }
    
    
}

``````