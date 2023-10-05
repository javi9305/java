
`````` java
 public static void main(String[] args) {
        //Se pide al usuario que proporcione un mes.
        System.out.println("Proporcione el mes");
        Scanner consola = new Scanner(System.in); //Creo un objeto de tipo Scanner y lo asigno a una variable de tipo Scanner.
        var mes = Integer.parseInt(consola.nextLine()); //se escribe el numero de mes y es convertido de String a entero

      var estacion = "Estacion desconocida"; //Creo una variable  asignandole una cadena la cual sera usada en cada caso.
      //el numero de mes otorgado por el usuario se verifica con el switch hasta encontrar el que el usuario tecleo y dependiendo sea el caso se imprimira una cadena.
        switch (mes) {
            case 1:     //tambien puede colocarse asi: case 1: case 2: case 12:
            case 2:                               // estacion = "Invierno";
            case 12:                              //   break; 
                estacion = "Invierno";
                break;
            case 3:
            case 4:
            case 5:
                estacion = "Primavera";
                break;
            case 6:
            case 7:
            case 8:
                estacion = "Verano";
                break;
            case 9:
            case 10:
            case 11:
                estacion = "Otonio";
                break;
           
        }
        System.out.println("estacion = " + estacion);














`````