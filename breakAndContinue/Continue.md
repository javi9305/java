
`````` java

public static void main(String[] args) {
        
        for (var contador = 0; contador < 3; contador++) {
            //si el numero no es un numero par.
            if (contador % 2 != 0) {
                // detener únicamente la iteración actual y saltar a la siguiente
               continue;//ir a la siguiente iteracion del ciclo for.
                
            }
             System.out.println("contador = " + contador);

        }
    }

    ``````