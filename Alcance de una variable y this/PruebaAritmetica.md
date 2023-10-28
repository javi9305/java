
`````` java
    public static void main(String[] args) {
  
       
       //Variables local, solamente se van a poder acceder dentro de este metodo
       int operandoA = 6;
       int operandoB = 2;
       
       //Creamos un objeto de la clase Aritmetica enviando argumentos
       //Usamos las variables locales para inicializar nuestro objeto aritmetica.
       Aritmetica objeto1 = new Aritmetica(operandoA,operandoB);
       
       //Imprimimos los valores de los operandos
        System.out.println("operandoA = " + operandoA);
        System.out.println("operandoB= " + operandoB);
        
        /*
        Estamos utilizando nuestras variables locales para inicializar nuestro objeto aritmetica,
        posteriormente nuestro objeto aritmetica con los valores de las variables locales recibidas
        inicializa los atributos de la clase.
        
        Clase Aritmetica
        
        public Aritmetica(int arg1, int arg2){
         a = arg1;
         b = arg2;
        }
        
        ya que hemos inicializado los atributos del objeto aritmetica, entonces podemos a mandar 
        a llamar los metodos sumar,restar, etc.
        
        y tambien pudimos observar que podemos imprimir  y acceder a las variables locales, si estamos dentro
        del mismo metodo donde se han definido estas variables(operandoA y operandoB).
        
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