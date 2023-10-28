

- Un constructor nos permite inicializar los valores de nuestra clase y ademas reservar espacio en memoria
para que se pueda crear un objeto/instancia de nuestra clase aritmetica

- Existen varios tipos de constructores que podemos tener en nuestra clase , el primer tipo de constructor es el vacio.

- El constructor es un metodo especial en java, ya que unicamente solo se puede mandar a llamar este metodo cuando se esta creando el objeto. No se puede mandar a llamar un metodo de tipo constructor  posterior a la creacion del objeto.

- Si no definimos un constructor en nuestra clase de manera explicita, entonces el compilador de java va a agregar por default el constructor vacio, de lo contrario no podriamos crear el objeto aritmetica. Siempre y cuando no tengamos otro tipos de constructores que reciban argumentos, si definimos un constructor con argumentos , entonces ya no se va agregar de manera automatica el constructor vacio por el compilador
ahora nosotros somos responsables de agregarlo a nuestra clase es decir de definirlo de manera explicita.


- la diferencia entre un metodo y un constructor, es que no regresa ningun tipo de dato(ni un void, ni un int, float etc).


- Esto no seria posible: aritmetica.Aritmetica();

ya que el constructor unicamente se puede mandar a llamar para crear el objeto es decir que debe ir en conjunto con la palabra new
Una vez se ha creado el objeto ya no se puede mandar a llamar a los constructores




`````` java
public static void main(String[] args) {

        //Crear objeto de tipo aritmetica
        /*
        En resumen
        Tenemos nuestra clase Aritmetica que es la plantilla y tenemos new Aritmetica(), que lo que estamos
        haciendo es mandar a llamar al constructor que esta definido en nuestra plantilla, y lo que va a hacer 
        este constructor es crear un objeto solicitando espacio de memoria para crear este objeto (new Aritmetica) y ese objeto
        se creo en el espacio de memoria que nos ha indicado java y posteriomente la variable aritmetica apunta
        al objeto que se ha creado en el espacio de memoria que no ha proporcionado el constructor vacio.
        */

        Aritmetica aritmetica = new Aritmetica(); //mandamos a llamar al constructor vacio.
        
        //Se realiza la suma y se asigna a la variable resultado.
        int resultadoSuma = aritmetica.sumar(5, 2); 
        int resultadoResta = aritmetica.restar(4, 2);
        int resultadoMultiplicacion = aritmetica.multiplicar(8, 5);
        double resultadoDividir = aritmetica.dividir(10, 3);
        
        //Impresion de resultados
        System.out.println("Resultado = " + resultadoSuma);
        System.out.println("Resultado = " + resultadoResta);
        System.out.println("Resultado = " + resultadoMultiplicacion);
        System.out.println("Resultado = " + resultadoDividir);
    }


    ``````
