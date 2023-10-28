`````` java


public class Aritmetica {
    /*
    el operador this se puede usar dentro de una clase, ya que cuando creamos
    un objeto en este caso de la clase Aritmetica (new Aritmetica -> esta en la clase PruebaAritmetica),
    en automatico el compilador de java crea una variable llamada this y lo que hace
    es apuntar al objeto que se esta creando.
    
    nos va a servir para poder acceder a los atributos y metodos de la clase,
    en el momento en que se esta realizando  la ejecucion de codigo de nuestra clase
    por lo tanto en el constructor se puede usar el this por ejemplo this.a y this.b.
    
     Si hacemos esto: 
     public Aritmetica(int a, int b){
       a = a;
       b = b; 
   
    }
    
    En este caso el argumento que estamos recibiendo en lugar de asignar el valor hacia el atributo de nuestra clase
    se esta utilizando el mismo argumento que estamos recibiendo para asignar el valor a si mismo, esto provoca una ambiguedad.
    para romper esta ambiguedad entonces tenemos que utilizar el operador this
    
    
    */
    int a;
    int b;
    
     //Constructor
    public Aritmetica() {
        System.out.println("Ejecutando constructor vacio");
    }
    
    public Aritmetica(int a, int b){
        this.a = a;
        this.b = b;
        System.out.println("Ejecutando constructor con dos argumentos");
    
    }
    
    
    
    public int sumar() {
        return this.a + this.b;
    }
    
    public int restar(){
        return this.a - this.b;
    } 
    public int multiplicar(){
        return this.a * this.b;
    }
    
    public int dividir(){
     return this.a/this.b;
    }
}

``````
Entrando en modo debug

![this1](/imagenesjava/this1.png "this1")

Damos en step into (f7)

![this2](/imagenesjava/this2.png "this2")



Entramos al detalle del objeto aritmetica

Podemos observar que en automatico el compilador a creado esta variable llamada this, a travez de la 
variable this que se ha creado es que podemos hacer referencia al objeto aritmetica que se ha creado tambien
en la direccion de memoria.

es decir como estamos dentro de la clase aritmetica y se ha creado un objeto en memoria por ejemplo 0 x 333 y por lo tanto this apunta al objeto que se ha creado en la direccion de memoria 0 x 333.

una vez que salimos de la ejecucion de esta clase entonces el operador this cambia y apunta a otra clase.

el operador this es de tipo aritmetica ya que esta apuntando a un objeto de tipo aritmetica.

podemos observar que el operador this puede acceder a los atributos de la clase.



le asignamos los argumentos a y b a los atributos de la clase this.a y this.b

![this3](/imagenesjava/this3.png "this3")