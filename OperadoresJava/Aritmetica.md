
`````` java

public class Aritmetica {

   //Metodo principal main
    public static void main(String[] args) {

        int a = 3, b = 2;  //Declaracion de variables enteras asignandoles un valor a cada una.
        
        var resultado = a + b; //sumo las variables a y b  asignadolas a una nueva variable llamada resultado.
        
        //Impresion cada uno de los resultados de suma,resta,multiplicacion,division y modulo.
        System.out.println("resultado suma = " + resultado);

        resultado = a - b;
        System.out.println("resultado resta = " + resultado);

        resultado = a * b;
        System.out.println("resultado multiplicacion = " + resultado);

        resultado = a / b;
        System.out.println("resultado de la division = " + resultado);

        resultado = a % b;
        System.out.println("resultado modulo = " + resultado);


        var resultado2 = 3.0 + b; //Da como resultado 1.5, al igual si se le pone 3D -> d significa double
        /*
         No es lo mismo utilizar un tipo float a decir que un valor es de tipo flotante. si decimos que un valor es de tipo flotante
         significa que tiene punto decimal en cambio si decimos que un tipo float  solamente nos estamos refiriendo al tipo de java.

         Se refiere a que al decir valor flotante puede ser cualquier número decimal (1.5, 2.0, 3.25, 90.7, 8.976.745.843) cualquier valor de estos son flotantes mientras que en java se usa el termino float para referirse al tipo de dato que solo puede almacenar 32 bits.
        
        */


        //es par o impar
        if (a % b == 0) { //si el resultado es 0 sera true y entrara al if
            System.out.println("Es un numero par");
        } else { //de lo contrario no entrara al if.
            System.out.println("Es un numero impar");
        }
        
    }
    
}

``````