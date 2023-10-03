`````` java

 public static void main(String[] args) {

        //Declaracion de variables asignandoles un valor a cada una.
        var a = 10;
        var valorMinimo = 0;
        var valorMaximo = 10; 
        
        //Evaluacion de las variables usando operadores relaciones y el uso del Condicional AND
        var resultado = a >= 0 && a <= 10;

        //verifica si el resultado es true esta dentro del rango que se esta evaluando.
        if (resultado) {

            System.out.println("Dentro del rango");
            //En caso contrario esta fuera del rango que se esta evaluando.
        } else {

            System.out.println("Fuera del rango");
        }

        //Declaracion de variables de tipo Boolean
        var vacaciones = false;
        var diaDescanso = false;
       //Verifica las dos variables usando el Condicional OR
        if (vacaciones || diaDescanso) { //si los dos resultados son falsos, regresa el valor de falso y ya no se ejecutaria el if.
            System.out.println("Padre puede asistir al juego del hijo");
        } else {
            System.out.println("El padre esta ocupado");
        }

    }



`````` 