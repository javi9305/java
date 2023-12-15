#### Clase Chip

`````` java

    //Atributos
  private String empresa;
  private int numero;

  //Constructor con 2 argumentos
    public Chip(String empresa, int numero) {
        //Asignando los argumentos.
        this.empresa = empresa;
        this.numero = numero;
    }

    public void mostrar(){
        System.out.println("Empresa: " + empresa);
        System.out.println("Numero de cel: " + numero);
    }

`````` 

#### Clase Bateria

`````` java

 //Atributos
    private int mAh;
    private String marca;
    
    //Constructor recibiendo 2 argumentos
    public Bateria(int mAh, String marca) {
        //Asignando los argumentos.
        this.mAh = mAh;
        this.marca = marca;
    }
  
    public void mostrar(){
        System.out.println("Cantidad de mAh: " + mAh);
        System.out.println("Marca: " + marca);
    }

``````


#### Clase SmartPhone

`````` java
//Atributos
    private String modelo;
    private Bateria bateria; //atributo de tipo Bateria
    private int nroChips; 
    private Chip[] chips;  //atributo de tipo Chip
    
    
    //constructor

    public SmartPhone(String modelo, int cantMAh, String marcaBateria) { //Recibo un argumento de tipo String y los 2 argumentos de la clase Bateria
        this.modelo = modelo;
        
        this.bateria = new Bateria(cantMAh, marcaBateria); //Creo objeto de tipo bateria
        this.nroChips = 0; //inicializo en 0.
        
        this.chips = new Chip[2]; //Creo un arreglo de tipo Chip
    }
    
    public void mostrar(){
        System.out.println("Modelo: " +modelo);
        bateria.mostrar();
        System.out.println("Nro Chips:" + nroChips);
        
        for (int i = 0; i < nroChips; i++) {
            chips[i].mostrar();
        }
    }
    
    public void agregarChip(Chip nuevoChip){
       if(nroChips < 2){
        chips[nroChips] = nuevoChip;
        nroChips++;
       }
    
    }

``````

#### Clase main

``````java
public static void main(String[] args) {
        //Creo un Objeto llamado cel de tipo SmarthPhone
        SmartPhone cel = new SmartPhone("A10PRO",3400,"Samsung");
        //Creo 2 Objetos de tipo Chip donde le paso 2 argumentos.
        Chip entel = new Chip("Entel",93821911);
        Chip tigo = new Chip("Tigo",3342222);
        
        //Objeto cel invoca al metodo agregarChip.
        cel.agregarChip(entel);
        cel.agregarChip(tigo);
        //Objeto cel invoca al metodo mostrar.
        cel.mostrar();
    }

``````