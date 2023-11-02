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

Usando el metodo toString para mejorar el codigo


Si nos damos cuenta cada vez que queremos imprimir los valores del objeto persona, estamos imprimiendo demasiadas lineas en consola, asi que con cada cambio que le hacemos al objeto, estamos mandando a llamar 3 veces la impresion la salida(a esto nos referimos con 3 veces: persona.getNombre, persona.getSueldo,persona.isEliminado).Para mejorar esto podemos hacer uso del metodo toString.

el metodo toString regresa una cadena con cada uno de los valores de cada atributo de la clase que estemos utilizando, en este caso la clase persona.


``````java


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

  /*
    public String toString(){
     
      return "nombre: " + nombre + ", sueldo: " + sueldo + ", eliminado: " + eliminado;
    
    }
    */
 //el ide nos puede ayudar a crear el metodo toString
    @Override //indica al compilador que se esta sobreescribiendo el metodo, ya que este metodo ya existe definido dentro de otra clase que es la clase Object.
    public String toString() {
        return "Persona{" + "nombre=" + nombre + ", sueldo=" + sueldo + ", eliminado=" + eliminado + '}';
    }
    
    
    
}

``````
