``````java
public class Persona {
    private int idPersona;
    private String nombre;
    private int edad;
    private static int contadorPersonas;
    
    private Persona(){
     /* super(); -> de manera implicita este constructor manda a llamar a 
     super en caso de que no lo hagamos de forma explicita es decir que lo 
     coloquemos de forma visible. */
    this.idPersona = ++contadorPersonas;
    
    }
    //Constructor completo - sobrecarga
    public Persona(String nombre, int edad){
       this(); //Accedemos al constructor vacio
       this.nombre = nombre;
       this.edad = edad;
       
    
    }

    public int getIdPersona() {
        return idPersona;
    }

  

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }

    public static int getContadorPersonas() {
        return contadorPersonas;
    }


    @Override
    public String toString() {
        return "Persona{" + "idPersona=" + idPersona + ", nombre=" + nombre + ", edad=" + edad + '}';
    }
    
    
}

``````