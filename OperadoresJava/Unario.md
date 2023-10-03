

`````` java

public static void main(String[] args) {
        //Declaracion de variables asignandoles un valor a cada una.

        //Operador unario.
       var a = 3;
       var b = -a; //invertir el signo
       //Impresion de variables 
        System.out.println("a = " + a);
        System.out.println("b = " + b);

         //Operador de inversion para tipos boolean. -> operador de complemento ya que a nivel de operaciones binarias funciona como un operador de complemento esto quiere decir,
         //que invierte el signo y pasa de 0 a 1.

        //Declaracion de variable booleana.
        var c = true;
        var d =!c;
        //Impresion de variable booleana.
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        



        //Incremento
        //1.preincremento (simbolo ++ antes de la variable)
        
        int e = 3;
         int f = ++e //primero usamos el operador del pre-incremento y luego la variable.
                     //el valor de la variable e, se va a incrementar en 1 y posteriormente se asigna este valor a la variable f. 
                     //se evalua primero lo del lado derecho es decir que la variable e ya vale 4 y se asigna a la variable f.
                     //primero se incrementa la variable y despues se usa su valor.
        System.out.println("e = " + e);
        System.out.println("f = " + f); 
      
        //2.postincremento (simbolo ++ despues de la variable)
        var g = 5;
        var h = g++;//primero se asigna el valor de la variable g a la variable h y se va a incrementar esta variable g hasta la siguiente vez que utilizemos esta variable.
                    //primero se utiliza el valor y despues se incrementa.
        System.out.println("g = " + g);//teniamos pendiente un incremento porque g valia 5 anteriormente.
        System.out.println("h = " + h);
        
        
        //Decremento
        //1.predecremento
        var i = 2;
        var j = --i;
        System.out.println("i = " + i); //ya esta decrementada
        System.out.println("j = " + j);
        
        //2.postdecremento
        var k = 4;
        var l = k--; //primero se usa el valor de la variable y queda pendiente un decremento.
        
        System.out.println("k = " + k);//tenia pendiente un decremento
        System.out.println("l = " + l);
       
        //Verificacion de que se realizo el postdecremento.
        l = k;
        System.out.println(l);
        
        
    }










`````` 