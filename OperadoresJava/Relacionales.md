
`````` java

public static void main(String[] args) {
        
        //Declaracion de variables asignandoles un valor a cada una.
        var a = 3;
        var b = 2;

        var g = a >= b; //mayor  que > o el mayor o igual >= , se esta comparando si a es mayor a b en caso de ser true se asigna el valor a g.
        System.out.println("g = " + g); //Imprime lo que contenga la variable g.

        //si el numero es par entra al if en caso contrario sera un numero impar y entrara al else. 
        if (a % 2 == 0) { //se evalua la expresion del lado izquierdo, posteriormente se evalua la expresion del lado derecho y finalmente se evalua toda la expresion (a%2 == 0), 
                          // regresa un resultado booleano.
            System.out.println("Es un numero par");
        } else {

            System.out.println("Es un numero impar");

        }
        //Declaracion de variables asignandoles un valor a cada una.
        var edad = 10;
        var adulto = 18;
        //Verifica si es un adulto o un menor de edad, segun su edad.
        if (edad >= adulto) {
            System.out.println("Es un adulto");
        } else {

            System.out.println("Es menor de edad");
        }
    }



``````