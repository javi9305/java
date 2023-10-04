
`````` java


   public static void main(String[] args) {
         //Se pide al usuario que proporcione un mes.
        System.out.println("Proporcione el mes");
        Scanner consola = new Scanner(System.in); //Creo un objeto de tipo Scanner y lo asigno a una variable de tipo Scanner.
        var mes = Integer.parseInt(consola.nextLine());//se escribe el numero de mes y es convertido de String a entero
  
      var estacion = "Estacion desconocida"; //Creo una variable  asignandole una cadena la cual sera usada dentro de cada if.
      //el numero de mes otorgado por el usuario sera verificado por cada uno de los if hasta encontrar el que el usuario tecleo.
      if (mes == 1 || mes == 2 || mes == 12){
         estacion = "Invierno";
      
      }
      else if (mes == 3 || mes == 4 || mes == 5){
      estacion = "Primavera";
      
      }
        
      else if (mes == 6 || mes == 7 || mes == 8){
      estacion = "Verano";
      
      }
      
      else if (mes == 9 || mes == 10 || mes == 11){
      estacion = "Otonio";
      
      }
        System.out.println("estacion = " + estacion);
        
    }





// Otra forma de pedir datos
 
        System.out.println("Proporcione el mes");
        var scanner = new Scanner(System.in); 
        /*
        La diferencia entre nextInt y nextLine es que nextLine incluye la lectura del caracter salto de linea, en cambio nextInt solamente
        lee el numero proporcionado pero no lee el caracter salto de linea, asi que si queremos volver a leer informacion de la consola
        entonces tendriamos que utilizar nextInt y aparte hacer una llamada al metodo next para que consuma el caracter de salto de linea.
        y entonces esto seria equivalente a realizar una llamada a nextLine, pero eso seria necesario unicamente si queremos leer mas de una vez
        informacion de la consola.
        
        nextInt de manera automatica regresa un entero y ya es necesario hacer la conversion de parseInt.

        */ 
        var mes = Integer.parseInt(consola.nextInt());


        `````` 