### Clase Documento

``````java
 private String titulo;
    private String cuerpo;

    public Documento(String titulo, String cuerpo) {
        this.titulo = titulo;
        this.cuerpo = cuerpo;
    }

    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getCuerpo() {
        return cuerpo;
    }

    public void setCuerpo(String cuerpo) {
        this.cuerpo = cuerpo;
    }

``````

### Clase Impresora

``````java
    private boolean estaEncendida;

 public void encender(){
     estaEncendida = true;
 }
    
   public void imprimir(Documento doc){ //parametro de tipo Documento (dependencia o uso)
    if(estaEncendida){
        System.out.println("Imprimiendo doc " + doc.getTitulo());
        System.out.println("****************");
        System.out.println(doc.getCuerpo());
        System.out.println("****************");
    }
    else{
        System.out.println("impresora apagada!");
    }
   } 

``````



### Clase Principal


``````java
    public static void main(String[] args) {
        Documento doc1 = new Documento("Prueba", "Este es un \ntexto de prueba");
        Impresora imp = new Impresora();
        
        imp.encender();
        imp.imprimir(doc1);
    }

``````


### ¿ Cuando ocurre la relacion ?

si nosotros afirmamos que una impresora "tiene" documentos o que se compone de un documento, estariamos en un error, porque para decir ello,
tendriamos que ir a la clase impresora y observar algun atributo o algunos atributos de tipo documento, sin embargo no existe.

Esto no implica de todas formas que documento e impresora no tengan relacion. ¿por que?

porque en la clase impresora se conoce la existencia de la clase documento, ya que en uno de sus metodos, aparece el tipo de dato documento, en
este caso particular se obtiene un documento via parametro, pero tambien pudimos haber generado un documento como variable local, haber devuelto un documento, entonces el tipo de retorno seria documento en lugar de void, pero no necesariamente el documento es un atributo. (si el retorno fuera documento, aqui tambien existiria una dependencia o uso)


Cuando tenemos este tipo de situaciones donde una clase conoce la existencia de la otra pero no necesariamente, teniendola como atributo, entonces estamos hablando
de una relacion de uso o dependencia, entre la clase impresora y documento, es una relacion un poco mas debil, pero es una relacion al fin al cabo, si nosotros movemos de paquete la clase documento o le cambiamos su nombre o la borramos, va a tener efectos en la clase impresora porque estamos conociendo su existencia.


### Diagrama uml


![umldependencia](/imagenesjava/umldependencia.png)



impresora depende de documento o impresora usa documento.




### Referencia

[Uso o Dependencia en java](https://www.youtube.com/watch?v=Mh_sgyDdir0)