
`````` java

public class EjemploEstatico {

    public static void main(String[] args) {
        Persona persona1 = new Persona("Juan");
        System.out.println(persona1);
        
        Persona persona2 = new Persona("Karla");
        System.out.println(persona2);
        
        //no se usa ningun objeto, sino usamos el nombre de la clase.
        System.out.println("contadorPersonas: " + Persona.getContadorPersonas());
    }
}

``````


Explicacion de codigo