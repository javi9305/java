
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
        else if(numero == 2){
        
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

    ``````