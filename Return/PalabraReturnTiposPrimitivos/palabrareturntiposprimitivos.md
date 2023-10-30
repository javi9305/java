

`````` java

 public static void main(String[] args) {
         sumarSinRetornarValor(3,6);
         int resultado = sumarRetornandoValor(0, 0);
         System.out.println("resultado sumar retornando valor = " + resultado);
    }

    /*
    En este caso no necesitamos utilizar la palabra return, en automatico si llegamos
    a nuestra ultima linea de nuestro metodo sin importar si agregamos la palabra return
    por default va a regresar al metodo que hizo la llamada(sumarSinRetornarValor(3,6)).
    es opcional agregar la palabra return.
    */
    private static void sumarSinRetornarValor(int a, int b) {
        System.out.println("El resultado de sumar sin retornar valor: " + (a + b));
    }
    /*
    el return no puede regresar varios valores, solo regresa un solo valor.
    si queremos regresar mas de un valor tendremos que utilizar un arreglo o una coleccion
    eso tambien corresponde a un valor,a un objeto de tipo array o de tipo colection.
    */
    private static int sumarRetornandoValor(int a, int b){
        if (a == 0 && b == 0){
            System.out.println("Debe proporcionar valores distintos de cero");
             return 0;
        }
        System.out.println("los valores proporcionados son distintos de cero");
        return a + b;
    }

`````` 