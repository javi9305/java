`````` java


package matrices;


public class EjemploMatricesPrueba {
    public static void main(String[] args) {
        //.1 Declaramos una matriz de int
        int edades[][];
        
        //2.- Instanciamos la matriz de int
        edades = new int[3][2];
        
        //3.- instanciar los valores de la matriz
        edades[0][0] = 30;
        edades[0][1] = 15;
        edades[1][0] = 20;
        edades[1][1] = 45;
        edades[2][0] = 5;
        edades[2][1] = 38;
        
        //4.Imprimir
        System.out.println("Matriz enteros indice 0 0:" + edades[0][0]);
        System.out.println("Matriz enteros indice 2 0:" + edades[2][0]);
        
        
        //1.Declarar e instanciar una matriz de objetos de tipo Persona
        Persona personas[][] = new Persona[1][2];
        
        //2.Inicializamos valores
        personas[0][0] = new Persona("Juan");
        personas[0][1] = new Persona("Karla");
        
        //3.Imprimir valores
        System.out.println("Matriz persona indice 0 0:" + personas[0][0]);
        System.out.println("Matriz persona indice 0 1:" + personas[0][1]);
        
        //controla los renglones
        for (int renglon = 0; renglon < personas.length; renglon++) {
            //controla las columnas
            for (int columna = 0; columna < personas[renglon].length; columna++) { //personas[renglon].length -> obtenemos el numero de columnas
                System.out.println("Matriz personas indice: " + renglon+ "- " + columna + ": " +personas[renglon][columna]); 
            }
        }
    }
}

``````

Asi se visualiza una matriz:


![matriz](/imagenesjava/matriz.png "matriz")









``````