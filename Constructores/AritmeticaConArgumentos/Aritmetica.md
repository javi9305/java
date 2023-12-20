`````` java

public class AritmeticaConArgumentos {
   
    int a;
    int b;
    
    
    
     //Constructor
    public AritmeticaConArgumentos(){
        
        System.out.println("Ejecutando constructor vacio");
    
    }
    
    /*
    Cuando mandemos a llamar a este constructor va a recibir estos valores que se le pasen al constructor en estos argumentos
    y ese valor se le va a asignar al atributo de nuestra clase.
    
    el constructor vacio se agrega de manera automatica, asi que si no tenemos ningun constructor en nuestra
    clase esto quiere decir que el compilador en automatico agrega el constructor vacio, obviamente no lo agrega 
    con ningun codigo y por lo tanto tampoco inicializa ningun atributo de nuestra clase, unicamente este 
    constructor vacio lo agrega el compilador para poder reservar espacio en memoria, pero no va a realizar 
    ningun otro codigo como es la inicializacion de variables,
    pero si nosotros agregamos un constructor diferente de vacio, como un constructor que recibe 2 argumentos, 
    entonces el compilador ya no va agregar en automatico el constructor vacio, por lo tanto nosotros somos 
    responsable de agregarlo.
      
    */
    //segundo contructor
    public AritmeticaConArgumentos(int arg1, int arg2){
    
        a = arg1;
        b = arg2;
        System.out.println("Ejecutando constructor con 2 argumentos");
    }
    
    
    //Metodo sumar que recibe 2 argumentos y regresa el resultado.
    public int sumar() {

        return a + b; 

    }

    ``````