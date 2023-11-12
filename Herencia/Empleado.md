`````` java


public class Empleado extends Persona{
    private int idEmpleado;
    private double sueldo;
    private static int contadorEmpleado;
    // Otra forma de asignar datos.
//    public Empleado(String nombre,char genero, int edad,String direccion,double sueldo){
//    super(nombre,genero,edad,direccion);
//     this.idEmpleado = ++contadorEmpleado;
//     this.sueldo = sueldo;
//    
//    }
    
    
   
    public Empleado(String nombre,double sueldo){
        
       /*
         Para poder crear el objeto empleado necesitamos terminar primero el objeto padre es decir Persona, por ello
         la primera llamada debe ser al constructor padre, en dado que no existe super(nombre), se manda a llamar
         al constructor de la clase padre sin argumentos, esto para que termine de crear el objeto de la clase padre
         y posteriormente regresa a construir el objeto de la clase hija. */
      super(nombre);
      this.idEmpleado = ++contadorEmpleado;
      this.sueldo = sueldo;
    }

    public int getIdEmpleado() {
        return idEmpleado;
    }

 
    public double getSueldo() {
        return this.sueldo;
    }

    public void setSueldo(double sueldo) {
        this.sueldo = sueldo;
    }

    public static int getContadorEmpleado() {
        return contadorEmpleado;
    }

    @Override
    public String toString() {
        return super.toString() + "Empleado{" + "idEmpleado=" + idEmpleado + ", sueldo=" + sueldo + '}';
    }
  
    
    
}

``````