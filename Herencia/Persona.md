
`````` java

public class Persona {
    private String nombre;
    private char genero;
    private int edad;
    private String direccion;
    
    //Constructor vacio
    /*
      super lo que hace es mandar a llamar un constructor o metodos de la clase padre 
    Se debe definir este constructor vacio por 2 razones:
    1. Tenemos constructores con argumentos y ya no se crea el contructor de forma automatica.
    2. Porque la clase Cliente tiene el super de forma automatica, es decir 
       Si no tenemos  la llamada a super dentro del constructor de la clase hija, entonces en automatico
       se manda a llamar el constructor de la clase Padre vacio.*/
    public Persona(){
    
    }
    //Constructor con 1 argumento
    public Persona(String nombre){
      this.nombre = nombre;
    }
    
    
    //Constructor completo (Recibiria los argumentos que tenemos comentado en la clase Empleado)
    public Persona(String nombre, char genero, int edad,String direccion){
      this.nombre = nombre;
      this.genero = genero;
      this.edad = edad;
      this.direccion = direccion;
    
    }

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public char getGenero() {
        return genero;
    }

    public void setGenero(char genero) {
        this.genero = genero;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }

    public String getDireccion() {
        return direccion;
    }

    public void setDireccion(String direccion) {
        this.direccion = direccion;
    }

    @Override
    public String toString() {
        return "Persona{" + "nombre=" + nombre + ", genero=" + genero + ", edad=" + edad + ", direccion=" + direccion + '}';
    }
    
    
    
}
``````