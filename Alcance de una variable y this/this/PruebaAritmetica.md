`````` java

public static void main(String[] args) {
  
       
       //Variables local, solamente se van a poder acceder dentro de este metodo
       int operandoA = 6;
       int operandoB = 2;
       
     
       Aritmetica objeto1 = new Aritmetica(operandoA,operandoB);
       
       //Imprimimos los valores de los operandos
        System.out.println("operandoA = " + operandoA);
        System.out.println("operandoB= " + operandoB);
           
        
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