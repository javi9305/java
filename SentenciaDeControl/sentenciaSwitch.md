`````` java

public static void main(String[] args) {
        //Declaracion de variables.
        var numero = 2;  //Asigno un numero a la variable numero.
        var numeroTexto = "valor desconocido"; //Asigno una cadena a la variable numeroTexto.
//El switch evalua el numero segun los casos.
        switch (numero) {
            case 1:
                numeroTexto = "Numero uno";
                break; //Rompe el caso para que no continue con los demas casos.
            case 2:
                numeroTexto = "Numero dos";
                break;
            case 3:
                numeroTexto = "Numero tres";
                break;
            case 4:
                numeroTexto = "Numero cuatro";
                break;
            default:
                numeroTexto = "Caso no encontrado";

        }
        
        System.out.println("numeroTexto = " + numeroTexto); //Imprime el valor de la variable numero.  
    }



`````` 