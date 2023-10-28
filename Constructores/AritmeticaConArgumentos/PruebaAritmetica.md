
`````` java

 public static void main(String[] args) {
        
     
        Aritmetica1 aritmetica = new Aritmetica1(); 
        
        //Segunda forma de inicializar los atributos.
        //Colocar en comentarios estas 2 lineas de codigo para usar la primera forma que esta en la clase Aritmetica.
        aritmetica.a = 10;
        aritmetica.b = 3;
        
        //Se realizan las operaciones de suma.
        int resultadoSuma = aritmetica.sumar(); 
     
        
        //Se imprime los resultados correspondientes.
        System.out.println("Resultado = " + resultadoSuma);  
        
       /*
        ¿Para que utilizamos los constructores con argumentos?
        los utilizamos para inicializar los atributos de nuestra clase desde el momento
        de la creacion del objeto y no hacer esto:
        
       Aritmetica1 aritmetica = new Aritmetica1(); 
      
        aritmetica.a = 10;
        aritmetica.b = 3;
        
        Asignar valores posteriormente a la creacion del objeto, en java es comun que asignemos
        los valores desde el momento de la creacion del objeto es decir que vamos a utilizar
        el constructor  para asignar valores desde el momento de la creacion del objeto.
        */
       AritmeticaConArgumentos aritmetica2 = new AritmeticaConArgumentos(4, 2);
         System.out.println("Resultado2 = " + aritmetica2.sumar());
    }

    ``````