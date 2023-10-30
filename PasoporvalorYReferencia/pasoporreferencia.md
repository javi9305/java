`````` java

 public static void main(String[] args) {
        Persona persona = new Persona();
        
        persona.cambiarNombre("Juan");
        System.out.println("Valor nombre: " + persona.obtenerNombre());
        /*
        Paso por referencia
        Esto quiere decir que desde otros metodos podemos cambiar los valores
        de los atributos del objeto al cual estamos apuntando, a diferencia
        de los tipos primitivos en el cual unicamente se pasa una copia del valor
        y no se pueden modificar los valores desde los otros metodos cuando
        trabajamos con objetos esto es diferente.
        */
        
        /*
        lo que estamos pasando en la llamada de este metodo es unicamente
        la referencia del objeto al cual esta apuntando es decir la variable persona
        esta apuntando al objeto persona (new Persona)(es decir la referencia que tiene la variable persona).
        */
        modificarPersona(persona); //Debe ser un metodo estatico para que se pueda mandar a llamar.
        
        System.out.println("valor nombre modificado: " + persona.obtenerNombre());
      
             
    }

    //va a modificar el valor del atributo nombre del objeto que hemos pasado como referencia
   private static void modificarPersona(Persona personaArg) {
       personaArg.cambiarNombre("Carlos");
    }    

``````




explicacion del codigo

![pasoreferencia1](/imagenesjava/pasoreferencia1.png "pasoreferencia1")


![pasoreferencia2](/imagenesjava/pasoreferencia2.png "pasoreferencia2")

Lo que vamos a hacer es pasar esta referencia 0x237 a la variable PersonaArg en el método modificarPersona, después la variable PersonaArg va a apuntar al mismo objeto en la dirección de memoria 0x237, tanto la variable persona y PersonaArg están apuntando al mismo objeto
Asi que ambas variables pueden observar el valor del atributo nombre que es juan, pero como en la línea de código estamos accediendo al método cambiarNombre , en este caso la variable PersonaArg  va a cambiar el valor de juan a Carlos, pero ambas variables siguen apuntando al mismo objeto, asi que ambas variables van a ver el valor de Carlos y posteriormente cuando termina el método modificarPersona, se elimina la variable PersonaArg, pero la variable persona continua apuntando al objeto en la referencia 0 x 237.
