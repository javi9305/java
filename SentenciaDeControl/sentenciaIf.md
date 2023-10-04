



`````` java

public static void main(String[] args) {

        var condicion = true; //variable de tipo boolean.
         //si la condicion es verdadera imprimira el texto dentro del if.
        if (condicion) {
            System.out.println("Condicion verdadera");
            //De lo contrario imprimira el otro texto que contiene else.
        } else {

            System.out.println("Condicion falsa");
        }

        //Declaracion de variables de tipo entero.
        var numero = 4;
        var numeroTexto = "Numero desconocido";
        
        //Verifica el numero en cada uno de los if hasta que la condicion de algun if se cumpla.
        if (numero == 1){
        
            numeroTexto = "Numero uno";        
        }
        //sino si (numero == 2)
        else if(numero == 2){ //se usa else if para ligar el if del principio, si solo se pone if, if se estaria usando de manera separada.
        
            numeroTexto = "Numero dos";
        }
        else if (numero == 3){
           numeroTexto = "Numero tres";
        
        }
        else if (numero == 4){
           numeroTexto = "Numero cuatro";
        }
        
        else{
            System.out.println("Numero no encontrado");
        }
        
        System.out.println("numeroTexto = " + numeroTexto);
        
        
        
    }


/* Es importante no usar los if de manera aislada ya que si se usa de esta forma, nuestro programa trabaja demas.
   ya que cada if que detecta tiene que revisar nuevamente la condicion.

   aqui revisa si el numero fue igual a 1


   si fue igual a 2


   si fue igual a 3


   si fue igual a 4

   en toda las ocasiones revisa esta condicion.




   en cambio si utilizamos else if entonces lo que sucede que una vez que encuentre la condicion ya no evalua ninguna de las otras condiciones, solamente
   esta buscando una condicion y una vez que la encuentra todo lo demas lo va a omitir. por ello es importante que liguemos nuestros casos con if, else if.
   y si agregamos otro if es porque ya es otra condicion o es otro codigo que queremos evaluar.


*/













    
    ``````
