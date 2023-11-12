`````` java


import java.util.Date;


public class Cliente extends Persona{
    private int idCliente;
    private Date fechaRegistro;
    private boolean vip;
    private static int contadorClientes;
    
    /*
    Podemos observar que aqui no tenemos una llamada al metodo super de forma visual
    sino que se va a mandar a llamar de manera automatica el constructor super vacio
    de la clase padre Persona antes del this.idCliente, por ello debemos tener definido el constructor
    se va a dirigir aqui:
    
    public Persona(){
    
    }
    
    */
    public Cliente(Date fechaRegistro,boolean vip){
       this.idCliente = ++contadorClientes;
       this.fechaRegistro = fechaRegistro;
       this.vip = vip;
    }

    public int getIdCliente() {
        return idCliente;
    }

  

    public Date getFechaRegistro() {
        return fechaRegistro;
    }

    public void setFechaRegistro(Date fechaRegistro) {
        this.fechaRegistro = fechaRegistro;
    }

    public boolean isVip() {
        return vip;
    }

    public void setVip(boolean vip) {
        this.vip = vip;
    }

    public static int getContadorClientes() {
        return contadorClientes;
    } 

    @Override
    public String toString() {
        return super.toString() + "Cliente{" + "idCliente=" + idCliente + ", fechaRegistro=" + fechaRegistro + ", vip=" + vip + '}';
    }
    
    
    
}


`````` 

















`````` 