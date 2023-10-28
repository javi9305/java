


`````` java

public static void main(String[] args) {
        
     
        Aritmetica1 aritmetica = new Aritmetica1(); 
        
        /*
        una vez que se ha creado el objeto tambien se puede modificar los valores directamente
        pero esto ya no seria a traves del constructor sino con la variable que apunta al objeto
        que se ha creado.
        
        Esta asignacion de valores de los atributos ya no lo hizo el constructor pero
        lo estamos haciendo con la variable(arimetica) que apunta al objeto que se ha creado.
        (new AritmeticaConArgumentos())
        
        Esto no es una buena practica, acceder directamente a los atributos de nuestra clase.
        Se puede acceder directamente a los atributos de nuestra clase siempre y cuando se declaren
        los atributos en la clase AritmeticaConArgumentos.

        */
        //Segunda forma de inicializar los atributos.         
        aritmetica.a = 10;
        aritmetica.b = 3;
        
        //Se realizan las operaciones de suma,resta,multiplicacion y division y se asigna el resultado a las variables correspondientes.
        int resultadoSuma = aritmetica.sumar(); 
     
        
        //Se imprime los resultados correspondientes.
        System.out.println("Resultado = " + resultadoSuma);  
        
            
    }

    ``````