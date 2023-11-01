Este codigo es sin usar el encapsulamiento

`````` java
public class Persona {
String nombre;
double sueldo;
boolean eliminado;

public Persona(String nombre, double sueldo, boolean eliminado){
    
    //El acceder directamente a los atributos solo debe ser dentro de la misma clase.
    //por ello accedemos usando la palabra this para acceder a nuestra clase.
  this.nombre = nombre;
  this.sueldo = sueldo;
  this.eliminado = eliminado;
}
}

`````` 
Usando el encapsulamiento

`````` java

public class Persona {
    //Cuando ponemos en privados los atributos, estos se encapsulan.
private String nombre;
private double sueldo;
private boolean eliminado;

public Persona(String nombre, double sueldo, boolean eliminado){
    
    //El acceder directamente a los atributos solo debe ser dentro de la misma clase.
    
    ////El acceder directamente a los atributos solo debe ser dentro de la misma clase.
    //por ello accedemos usando la palabra this para acceder a nuestra clase.
    
  this.nombre = nombre;
  this.sueldo = sueldo;
  this.eliminado = eliminado;
}

//Metodos getter y setter
   public String getNombre(){
     return this.nombre;
   }
   
   public void setNombre(String nombre){
      this.nombre = nombre;
   }

    public double getSueldo() {
        return sueldo;
    }

    public void setSueldo(double sueldo) {
        this.sueldo = sueldo;
    }

    public boolean isEliminado() {//se usa is debido  a que el tipo booleano es mas bien una pregunta: ¿es eliminado?
        return eliminado;
    }

    public void setEliminado(boolean eliminado) {
        this.eliminado = eliminado;
    }


}

`````` 

