La política de cobro de una compañía telefónica es:
Cuando se realiza una llamada, el cobro es por el tiempo que esta dura, de
tal forma que los primeros cinco minutos cuestan 1 euro, los siguientes tres,
80 céntimos, los siguientes dos minutos a 70 céntimos y a partir del décimo minuto, 50 céntimos.
Además, se carga un impuesto de 3% cuando es domingo, y si es otro día, en turno de mañana 15% y en turno de tarde 10%.
Realiza un algoritmo para determinar cuánto debe pagar por cada concepto una persona que realiza una llamada.



`````` java

public static void main(String[] args) {
        String dia;
        int duracion;
        double costoLlamada;
        Scanner consola = new Scanner (System.in);
        
        
        System.out.println("Introduce el tiempo de la llamada");
        duracion = Integer.parseInt(consola.nextLine());
        
        System.out.println("Introduce el dia de la semana: ");
        dia = consola.nextLine();
        
        
        /*
        Entre los minutos 0 a 5, el cliente pagará 1 €
        Del minuto 6 a 8, el cliente pagará 0,80 €
        Del minuto 9 a 10, el cliente pagará 0,70 €
        A partir de los 11 minutos, el cliente pagará 0,50 €
        
        
        Con esta tarificación, el cliente pagará por la misma llamada de 
        11 minutos, un total de 3 €. Por tanto, las condiciones vendrían a 
        ser las siguientes:

        Si duracion > 10, coste = 3 € -> se suman 1 +0.80 + 0.70 + 0.50 = 3€  -> duracion 11 minutos.
        Si duracion > 8, coste = 2,50 € -> se suman 0.80 + 0.70 + 0.50 = 2,50€ - > duracion 10 minutos.
        Si duracion > 5, coste = 1,80 € -> se suman 0.80 + 1 = 1,80€ -> duracion 8 minutos.
        Si duracion <= 5, coste = 1 € -> duracion de 5 minutos o menos.
        
        
        
        
        */
        
          //Calculamos el precio base a pagar:
       if (duracion > 10){
           precioBase = 3;
       }
        
       else if (duracion > 8){
       
          precioBase = 2.5;
       } 
       
       else if (duracion > 5){
          precioBase = 1.80;
       
       }
       
       else{
          precioBase = 1;
       
       }
       
       //preguntamos dia y calculamos impuesto correspondiente.
       
       if(!dia.equals("domingo")){  //Abre primer if
           System.out.println("¿La llamada la realizo en horario de mañana o de tarde?");
           horario = consola.nextLine();
           
           if(horario.equals("mañana")){ //abre el segundo if
            impuesto = precioBase * 0.15;
           
           }
           
           else if(horario.equals("tarde")){
           impuesto = precioBase * 0.10;
           
           }
           else {
               //si el horario es incorrecto se da valor 0 al impuesto.
           impuesto = 0;
           } //cierre del segundo if
       
       }
       
       else{
       impuesto = precioBase * 0.03;
       } //cierre del primer if
       
       
    System.out.println("El precio total de la llamada es de " + (precioBase + impuesto) 
             + " siendo el precio base de " + precioBase + " y el impuesto a pagar " + impuesto);    
       
       
       
    } //cierre main
        
    ``````    
        
        
    