  
    
      Si no indicamos otra cosa, el constructor vacio lo que va a hacer
      es inicializar los valores de nuestras variables a y b, le asignara un valor
      por default dependiendo del tipo de dato por ejemplo si es tipo entero
      su valor por default es 0, si es un tipo objetc su valor por default es null.
    
    

    `````` java
   //Atributos de la clase
    int a;
    int b;
    
    
    
     //Constructor
    public Aritmetica1(){
        
    /*
    Primera forma de inicializar los atributos.
    el constructor se esta encargando de inicializar los valores de los  atributos de nuestra clase.
   
    a = 5;
    b = 3;
    
    */    
        System.out.println("Ejecutando constructor vacio");
    
    }
    
    
    
    //Metodo sumar que recibe 2 argumentos y regresa el resultado.
    public int sumar() {

        return a + b; //se utilizan los atributos de la clase.

    }

    ``````